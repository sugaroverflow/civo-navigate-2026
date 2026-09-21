## 2026-09-21T19:31:35Z - GitHub Pages routing fix

### Goal

Make every slide reachable in the deployed GitHub Pages deck, including keyboard navigation and direct links.

### Changes

- Changed `build:pages` to use a relative asset base (`./`) with `--router-mode hash`.
- Kept local development and ordinary builds on Slidev's default history routing.

### Decisions

GitHub Pages does not provide the SPA rewrite required by Slidev history routes. The deployed deck therefore uses hash URLs such as `/civo-navigate-2026/#/2`, which keep all slide navigation on the published `index.html`. Slidev 52.16 also prepends `BASE_URL` when generating an in-app slide path, so using `/civo-navigate-2026/` as both the router base and the deployment base duplicated it during navigation. A relative base keeps assets under the current repository path without adding that path to slide routes.

### Tradeoffs

Hash URLs are less visually clean than history URLs, but they work on GitHub Pages without a custom 404 fallback or another hosting layer.

### Risks

Future changes to the Pages build command must preserve both `--base ./` and `--router-mode hash`. Replacing the relative base with the repository path recreates the doubled-base/404 failure when advancing slides.

### Verification

- Reproduced the live failure in Playwright: slide 1 advanced to `/civo-navigate-2026/civo-navigate-2026/2` and rendered Slidev's 404 page.
- Confirmed that hash routing with `/civo-navigate-2026/` as `BASE_URL` was still insufficient: it advanced to `#/civo-navigate-2026/2` and rendered Slidev's 404 page.
- Built the relative-base variant and served it under the real `/civo-navigate-2026/` subpath.
- Verified with Playwright that Arrow Right advanced to `/civo-navigate-2026/#/2`, rendered the complete bio slide and headshot, and produced zero console errors.
- Live navigation will be rechecked after the final configuration is deployed.

### Demo Impact

The hosted deck can now be used for rehearsal and presenting without slide 2 failing immediately.

### Customer-Facing Context

This is a static-host routing constraint, not missing slide content or a broken asset.

### Next Recommended Step

After deployment, test slide 1 to slide 2, a direct slide URL, and presenter mode on the public Pages site.
