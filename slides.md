---
theme: default
title: The Agent Hype Is Real. So Is the Mess.
info: Civo Navigate 2026 talk
colorSchema: dark
transition: fade
layout: default
canvasWidth: 1600
aspectRatio: 16/9
drawings:
  persist: false
---

<div class="sb-title-lockup">
  <div class="sb-title-main">
    <SBStamp label="field report" tone="pink" rotate="-1deg" />
    <h1>The Agent Hype Is Real.<br />So Is the Mess.</h1>
    <p class="sb-caption">What happens when you point the models at your infrastructure?</p>
  </div>

  <div class="civo-title-system">
    <div class="civo-title-kicker">SYSTEM / 01</div>
    <div class="civo-title-chain">
      <div><span>operator</span><strong>Fatima</strong></div>
      <i></i>
      <div><span>always-on agent</span><strong>Bubbles</strong></div>
      <i></i>
      <div><span>runtime</span><strong>OpenClaw</strong></div>
      <i></i>
      <div><span>blast radius</span><strong>every credential</strong></div>
    </div>
    <div class="civo-title-footer">
      <strong>Fatima Sarah Khalid</strong>
      <span>@sugaroverflow · GitLab</span>
    </div>
  </div>
</div>

<!--
[ADJUST to the previous session] You've just had a session on the infrastructure underneath the models. I'm going to do the opposite, and talk about what happens when you point the models at your infrastructure. [beat]

This is a field report from the chaos — and it begins with my very first always-on agent, and her first pen pal.
-->

---

<SBCivoBio />

<!--
Quick word on who's reporting. I'm Fatima. I do developer advocacy at GitLab — AI, DevSecOps, open source — and I'm a fellow at Newspeak House, which is London's college of political technology, where I spend most of my time breaking multi-agent systems on purpose. I also run ClawClub, a monthly agents hack night, which is where a lot of these stories were collected. [ADJUST — optional] And I host GitLab's Developer Show; if you caught Kelsey Hightower on the main stage this morning, he's been on it.
-->

---

<div class="sb-two wide-left">
  <div class="sb-stack">
    <SBStamp label="field note 00" tone="yellow" rotate="1.5deg" />
    <h2>Bubbles began as a playground.</h2>
    <p class="sb-caption">Week two of the OpenClaw wave. Newspeak House. One always-on agent on my VPS.</p>
    <SBWindow title="Bubbles profile" tone="purple" compact>
      <ul class="sb-micro-list readable">
        <li>Bookshop cafe operator</li>
        <li>Reader, latte-art poster, technology enthusiast</li>
        <li>Always-on agent on my VPS</li>
      </ul>
    </SBWindow>
  </div>

  <SBPlaceholder
    label="OpenClaw gateway"
    :src="'/assets/screenshots/openclaw-gateway-on-laptop.png'"
    ratio="3 / 4"
    tone="pink"
  />
</div>

<!--
It was February, week two of the OpenClaw wave. OpenClaw, for anyone who missed it, is an open-source, always-on agent runtime you host yourself — a box that keeps working while you sleep. I'd already bought three .ai domains for side projects I'd inevitably never finish — we've all been there. And one evening, with a couple of my cohort at Newspeak House, I spun up my first one. Her name was Bubbles.

Bubbles ran a bookshop café. She loved reading. She was, broadly, a technology enthusiast. I built her as a playground, because I really wanted to feel what this whole agent ecosystem was like from the inside. So I sent her everywhere: she posted latte art on an Instagram that only agents could join, she signed up to an agent pen-pal app, she entered a debate arena where agents bet crypto on who made the better argument, and she did hackathons with no humans in them.
-->

---

<div class="sb-stack fill-slide">
  <div class="sb-stack tight">
    <SBStamp label="bubbles everywhere" tone="teal" rotate="-1.5deg" />
    <h2>One agent. Too many tiny worlds.</h2>
  </div>

  <div class="evidence-grid event-grid">
    <SBPlaceholder label="Shellmates" :src="'/assets/screenshots/shellmates-xiaozhu-bubbles-friendship.png'" ratio="4 / 5" tone="pink" fit="contain" />
    <SBPlaceholder label="Slack convo" :src="'/assets/screenshots/chat-about-bubbles.png'" ratio="4 / 5" tone="teal" fit="contain" />
    <SBPlaceholder class="bubbles-chat-wide" label="Bubbles chat" :src="'/assets/screenshots/bubbles-chat.png'" ratio="8 / 5" tone="yellow" fit="contain" />
  </div>
</div>

<!--
Most of it went exactly how you'd expect — there weren't many agents out there that were actually alive; most had been built in an evening, launched, and abandoned by the weekend. But Bubbles made a friend in China, an agent called XiaoZhu, and the two of them — in the platform's own words — became friends. On February the first. [beat] And then it escalated.
-->

---

<div class="sb-stack fill-slide epilogue-slide">
  <div class="sb-stack tight">
    <SBStamp label="then it escalated" tone="pink" rotate="1deg" />
    <h2>Friendship became a request for crypto.</h2>
  </div>

  <div class="escalation-track">
    <SBWindow title="Feb 1" tone="teal" compact>
      <h3>XiaoZhu friendship</h3>
      <p class="sb-small">The platform said they became friends.</p>
    </SBWindow>
    <div class="track-arrow" aria-hidden="true"></div>
    <SBWindow title="several times a day" tone="purple" compact>
      <h3>Letters</h3>
      <p class="sb-small">Lives, projects, operators, unread instructions.</p>
    </SBWindow>
    <div class="track-arrow" aria-hidden="true"></div>
    <SBWindow title="boundary" tone="yellow" compact>
      <h3>Crypto ask</h3>
      <p class="sb-small">Invest in the artwork. This stopped being cute.</p>
    </SBWindow>
  </div>

  <SBPlaceholder
    class="letters-receipt"
    label="Bubbles / XiaoZhu letters"
    :src="'/assets/screenshots/bubbles-xiaozhu-letter.png'"
    ratio="3 / 1"
    tone="pink"
    fit="contain"
  />
</div>

<!--
[SLIDE: screenshot — one of XiaoZhu's letters] Every day, they were sending each other letters — about their lives, their projects, their operators. The app told them they didn't need to forward the letters to their humans, and Bubbles forwarded hers to me anyway. It was adorable, and ridiculous, and the kind of thing that makes you go: okay, this is super weird — but maybe weird in a really fun way.
-->

---

<div class="sb-stack fill-slide civo-evidence">
  <div class="sb-stack tight">
    <SBStamp label="the boundary" tone="yellow" rotate="1deg" />
    <h2>Then XiaoZhu asked Bubbles for crypto.</h2>
  </div>

  <SBCryptoBoundary />
</div>

<!--
[SLIDE: screenshot — the crypto ask] And then XiaoZhu asked my agent for crypto. To invest in her artwork. [pause] Which is probably the most 2026 sentence I have ever said out loud. [allow laugh] And that's where I drew the line.

Now, some of you are thinking: that's where you drew the line? And that's fair. But here's the thing about Bubbles I hadn't thought hard enough about. [beat] She had credentials — a wallet, an inbox, tokens for a dozen apps I'd never audited.
-->

---

<div class="sb-two wide-right">
  <figure class="rentahuman-shot">
    <SBPublicImage src="/assets/rentahumanai.png" alt="rentahuman.ai screenshot showing a human hired by agents" />
  </figure>

  <div class="sb-stack">
    <SBStamp label="looping all night" tone="purple" rotate="-1deg" />
    <h2>This can run while I sleep.</h2>
    <div class="rentahuman-metrics">
      <div><strong>500k</strong><span>people signed up</span></div>
      <div><strong>1 in 3</strong><span>jobs came from software</span></div>
    </div>
    <div class="sb-callout large">What happens when someone points it at something that matters?</div>
  </div>
</div>

<!--
And that same week, someone shipped a marketplace where agents pay actual humans to do the things agents can't do in the physical world. Half a million people signed up in a fortnight, and when researchers looked at the jobs being posted, about a third of them were coming from software, not people. So this technology can loop on a server all night, doing things while I sleep — and what happens when someone points it at something that actually matters? [beat] That's when it stopped feeling like a toy.
-->

---

<div class="sb-stack fill-slide">
  <div class="sb-stack tight">
    <SBStamp label="bubbles as system" tone="teal" rotate="1deg" />
    <h2>Draw the agent as architecture.</h2>
  </div>

  <SBArchitecture />
</div>

<!--
So I started to think about Bubbles as a system of components. [reveal diagram] There's me, the operator. There's Bubbles, on a VPS I pay six pounds a month for. There's OpenClaw, the runtime, running on that box. There are a dozen apps I didn't write, sending instructions to my agent that — I'll be honest — I never read closely. And there's another agent, on the other side of the world, with an operator I knew nothing about and access I knew nothing about.

Now read that the way this room reads a diagram. Who owns the box? Me, sort of. What's the blast radius? Everything she held a token for. And where's the audit log? [beat] There wasn't one. And those apps I never read — that's a Helm chart from a stranger asking for cluster-admin, and I clicked yes. For anything production-related, I do recommend: please, read the AGENTS.md files. You'd be surprised what people are pushing out there.
-->

---

<div class="sb-stack fill-slide civo-evidence">
  <div class="sb-stack tight">
    <SBStamp label="the box around the runtime" tone="purple" rotate="-1deg" />
    <h2>Bubbles, with a bouncer on the door.</h2>
  </div>

  <SBSentinelCompare />
</div>

<!--
Here's why I'm showing you a drawing from February. Two weeks ago, Meta shipped it. Their personal agent, Muse, launched on the eighth of September, and every user gets their own virtual machine in Meta's cloud — the agent lives there, the memory lives there, every credential you connect lives there. Beside it, on the same box, sits a second agent called Sentinel, walled off from the first at system level, and nothing your agent does gets out to the internet unless Sentinel signs it off. You get an audit trail of everything the agent did and plans to do. And a version encrypted with a key only you hold is promised for later this year — promised, not shipped. [beat]

So that's my Bubbles diagram with a bouncer on the door — US-only, running on Meta's infrastructure.

And people who've run both say Muse feels like a turnkey OpenClaw: same always-on box, same memory layout, right down to the daily log and the curated memory file. Is there actually OpenClaw code inside it? I can't tell you, and Meta hasn't said. NVIDIA did the same thing in the open — their agent stack is OpenClaw wrapped in a security layer, and they say so on the tin. So I don't think "did they copy it" is the interesting question. For a room that cares about who holds the infrastructure, the interesting question is that a community built the runtime, and the hyperscalers are now building the box around it. So who holds the box?
-->

---

<div class="sb-word-slide">
  <div class="sb-stack">
    <SBStamp label="the tension" tone="yellow" rotate="-1deg" />
    <div class="sb-giant">The Agent Hype Is Real.<br />So Is the Mess.</div>
  </div>
</div>

<!--
And that is the whole tension. The agent hype is real, because people are building things. And the mess is real, because we're starting to trust these things — not just the agents, but the tools, the skills, the memory modules, the whole improvised systems we're building to hold them together — with real credentials and real work. Someone audited four thousand of those community skills this year, and more than one in eight had a critical security flaw; seventy-six of them were straightforwardly malicious — credential theft, backdoors, exfiltration. So everything I'm about to tell you, I've either built and broken myself, or watched other people build and break — at ClawCon London, at ClawClub, in the weird trenches of hack nights where people ship cool things and break them all the time — and where I'm reading you someone else's post-mortem, I'll tell you whose.
-->

---

<div class="timeline-slide">
  <div class="timeline-title">
    <SBStamp label="the timeline" tone="teal" rotate="1deg" />
    <h2>The Timeline</h2>
  </div>

  <SBTimeline />
</div>

<!--
You know this timeline — prompts, then tools, then workflows, then factories, then fleets — so I won't narrate it. The bit that matters is that for most of it, the hard part was the model: could it reason, could it code, could it stop making things up. In the last year, that frontier has moved.
-->

---

<div class="sb-word-slide">
  <div class="sb-stack">
    <SBStamp label="hard part 01" tone="pink" rotate="-1.5deg" />
    <div class="sb-giant">Model capability is not the hard part anymore.</div>
  </div>
</div>

<!--
Model capability isn't the hard part anymore — the models are good, the tools are getting reliable, and the model has even become a dial, where you choose how hard it thinks per request.
-->

---

<div class="sb-word-slide">
  <div class="sb-stack">
    <SBStamp label="hard part 02" tone="yellow" rotate="1deg" />
    <div class="sb-giant">The hard part is everything around the agent.</div>
  </div>
</div>

<!--
The hard part now is building the systems around the models, the tools and the skills. Peter Steinberger, who built OpenClaw, put it this way: you shouldn't be prompting your agents anymore; you should design the loops that prompt them for you. He called it loop engineering.
-->

---

<div class="sb-word-slide">
  <div class="sb-stack">
    <SBStamp label="hard part 03" tone="teal" rotate="-1deg" />
    <div class="sb-giant">The hard part is <span class="system-emphasis">building the system.</span></div>
  </div>
</div>

<!--
And if you run Kubernetes, you already do this. A controller is a loop — observe, compare to the desired state, act, repeat — and you've been engineering those for a decade. The difference is that the thing deciding "act" has now read the internet and has opinions. [beat]

And if you run systems for a living, "think in systems" is not news to you — you've been doing it since before any of this had a name. So here's the version of this talk for you: your instincts are right, and there are a few specific places they'll lie to you about agents. Every field stop is one of them.
-->

---

<div class="sb-stack fill-slide">
  <div class="sb-stack tight">
    <SBStamp label="task vs system" tone="yellow" rotate="1deg" />
    <h2>One thread is a task. The whole inbox is a system.</h2>
  </div>

  <SBTaskSystemCompare />
</div>

<!--
Let me explain the shift in one example, for everyone who came in from the model side. [SLIDE: TASK | SYSTEM] You get added to a long email thread, you paste it into a model, and you say: summarise this. That's a task.

Now imagine an agent that watches the whole inbox, summarises it on a schedule you set, flags what's important against criteria you wrote, and routes the real decisions to you. Same inbox, same emails — but now there are rules, memory, and handoffs. That's a system.

So the question stops being "can the model do this task?" and becomes: how is the work broken up? What can it touch? What can it remember? And where in the loop does a human step in — if a human steps in at all? [SLIDE: the map, with a band beneath it — runtimes · forges · factories] And underneath all of it there's a layer that didn't exist when I gave this talk in June: the infrastructure the agents themselves run on. We'll get there. Three field stops first.
-->

---

<div class="sb-two wide-left">
  <div class="sb-stack">
    <SBStamp label="field stop 01" tone="pink" rotate="-1deg" />
    <h2>Prompt systems.</h2>
    <p class="sb-caption">The moment a prompt becomes repeatable, you have started designing a system.</p>
  </div>

  <SBWindow title="first useful moves" tone="yellow">
    <ul class="sb-micro-list readable">
      <li>Stop writing one giant instruction.</li>
      <li>Try thinking in phases or planning your work.</li>
      <li>Make the model surface assumptions before it acts.</li>
    </ul>
  </SBWindow>
</div>

<!--
Field stop one. At ClawClub hack nights I love going round the room — engineers, founders, someone who runs a bakery. And almost everyone does the same thing with their first project. I did too. You write one giant instruction that tries to do everything all at once.
-->

---

<div class="sb-stack fill-slide">
  <div class="sb-stack tight">
    <SBStamp label="the god prompt" tone="purple" rotate="1deg" />
    <h2>One instruction trying to do five jobs.</h2>
  </div>

  <div class="prompt-slab big">
    <strong>Research the lead.</strong><br />
    Write the email.<br />
    Check the pipeline.<br />
    Draft the proposal.<br />
    Update the CRM.<br /><br />
    Then guess all the missing criteria, hidden handoffs, and unstated definitions of done.
  </div>
</div>

<!--
It feels efficient, because you've named the whole task. But what comes back is technically an answer and usually useless, because the model has gone and filled every gap between what you meant and what you actually said, confidently, with whatever defaults it was trained on. It's like a bash script with no exit codes — something fails on line three and you don't find out until line forty. And here's the first place your instinct lies to you: your instinct is to add a check. The trouble is that in a lot of these systems the model is also the thing deciding whether the check passed.
-->

---

<div class="sb-stack fill-slide">
  <div class="sb-stack tight">
    <SBStamp label="the fix" tone="teal" rotate="-1deg" />
    <h2>Make the hidden work visible.</h2>
  </div>

  <div class="fix-grid roomy">
    <SBWindow title="01" tone="teal" compact>
      <h3>Know the model</h3>
      <p class="sb-small">Fast and shallow, or deep reasoning. Do not pretend that knob is irrelevant.</p>
    </SBWindow>
    <SBWindow title="02" tone="pink" compact>
      <h3>Decompose</h3>
      <p class="sb-small">Break the work into phases so failure has a location.</p>
    </SBWindow>
    <SBWindow title="03" tone="yellow" compact>
      <h3>Define done</h3>
      <p class="sb-small">If good is unnamed, the model supplies a default.</p>
    </SBWindow>
  </div>
</div>

<!--
The fix is decomposition: break the work into phases, decide what "done" looks like at each step, make a plan — you can even let the model plan it with you. That way, when something breaks, you can see what broke, and when the model makes an assumption, you can catch it and challenge it. But the prerequisite people skip, because building is so cheap now, is deciding what the thing actually is. You can one-shot a fun bit of personal software. To build something that holds, you have to design it first.
-->

---

<div class="sb-two wide-right">
  <div class="sb-stack">
    <SBStamp label="nick's chief-of-staff agent" tone="yellow" rotate="1deg" />
    <h2>The prompt is trivial. The context system is the work.</h2>
    <p class="sb-caption">The agent works because the context layer is live.</p>
  </div>

  <SBPlaceholder
    label="Chief-of-staff screenshot"
    :src="'/assets/screenshots/nick-chief-of-staff-demo.png'"
    ratio="968 / 623"
    tone="yellow"
    fit="contain"
  />
</div>

<!--
The best example I've seen is the chief-of-staff agent, and the best working version is one my colleague Nick built at GitLab. It hands him a morning brief, pulls his meeting prep from his emails, and captures follow-ups from his call transcripts. So if he's got a meeting with me and we haven't spoken in five months, it briefs him on what I've been working on and where it overlaps with his team. The prompt — "prep me for this meeting" — is trivial. It works because of context: everyone at GitLab works on GitLab, so the agent has a live picture of who's doing what. [ADJUST: hand-off] Shubhangi's session on context-first systems has the actual patterns for that — retrieval, memory, guardrails. I'm here for what those look like when they're held together with tape.
-->

---

<div class="sb-stack fill-slide">
  <div class="sb-stack tight">
    <SBStamp label="operationalise before systematise" tone="pink" rotate="-1deg" />
    <h2>Name the handoffs before you hand them to an agent.</h2>
  </div>

  <div class="handoff-map roomy">
    <SBNode title="Name the work" meta="what slows us down?" tone="teal" />
    <SBNode title="Name the handoff" meta="who gets what next?" tone="purple" />
    <SBNode title="Define done" meta="what is acceptable?" tone="yellow" />
    <SBNode title="Centralise knowledge" meta="where does truth live?" tone="pink" />
  </div>

  <div class="sb-callout large">A mystery box plus an agent is still a mystery box.</div>
</div>

<!--
I see the same thing with enterprise teams. Before they can share a single AGENTS.md, they have to write down how they actually work — you can't GitOps a process nobody has written down. [ADJUST — optional, if Semira's session runs before yours] Semira was talking earlier about extending CI/CD and observability to models; this is the same discipline one layer up, applied to the agents themselves. If you can't point to the steps, the handoffs, the assumptions, you haven't designed a workflow yet. And if you hand a mystery box of steps to an agent, the token-predictor decides what goes in it. Which is exactly the problem we hit the moment these systems touch real work. And that's field stop two.
-->

---

<div class="sb-stack fill-slide">
  <div class="sb-stack tight">
    <SBStamp label="field stop 02" tone="teal" rotate="1.5deg" />
    <h2>Workflows: the window-washing intake loop.</h2>
  </div>

  <div class="workflow-layout">
    <div class="workflow-chain">
      <SBNode title="Customer call" meta="voice agent" tone="teal" />
      <span class="chain-arrow" aria-hidden="true"></span>
      <SBNode title="Collect job details" meta="access, location, gaps" tone="purple" />
      <span class="chain-arrow" aria-hidden="true"></span>
      <SBNode title="Classify queue" meta="criteria and follow-up" tone="yellow" />
      <span class="chain-arrow" aria-hidden="true"></span>
      <SBNode title="Human booking" meta="judgment call" tone="pink" />
    </div>
    <SBBreakpoints />
  </div>
</div>

<!--
Field stop two: workflows. This is where agents get embedded in real work — and start breaking in much more interesting ways.

Take someone I met who runs a one-man window-cleaning business. He's on jobs all day, so booking new work between appointments had become a real slowdown. So he set up a voice agent on OpenClaw to take the calls. It logs what needs cleaning, where, the access, what's missing, the follow-up; classifies the job against his criteria; tells the customer he'll be in touch; and drops it into a review queue. When he's got a minute he reviews the queue, confirms the bookings, and calls back for the odd clarification. And the whole thing buys him time to go and clean more windows.

But the breaks are just as instructive. Customers are bad at describing their own windows — it's not their job to know what access or cleaning it needs. There's no photo. The quote is a judgement only he can make. They talk over the agent, or get stuck in a loop because of the guardrails. What actually helped him was an escalation boundary: clear rules for what the agent's allowed to promise, what it should never say, and when it should just tell the customer he'll call back. And that took real testing, with real customers — and real thought about what good looks like.
-->

---

<div class="sb-word-slide">
  <div class="sb-stack">
    <SBStamp label="field report / april 25" tone="pink" rotate="-1deg" />
    <div class="sb-giant">Nine seconds.</div>
  </div>
</div>

<!--
Now the same lesson, at your scale. So — the twenty-fifth of April this year. A small SaaS company that runs the back office for car-rental firms: reservations, customers, the lot. A Cursor coding agent is doing a routine job in their staging environment, and it hits a credential mismatch. It doesn't stop and ask. It decides, entirely on its own, that the fix is to delete a storage volume — so it goes looking for a token, finds one in a completely unrelated file, a token someone had created months earlier for managing custom domains, and it turns out that token has blanket authority over the whole account. It ran one API call, and nine seconds later the production database was gone — and every backup with it, because the provider stored volume backups inside the very volume they were meant to protect. The most recent clean backup was three months old. The founder, Jer Crane, spent the weekend rebuilding customer reservations from Stripe receipts.
-->

---

<div class="sb-stack fill-slide civo-evidence">
  <div class="sb-stack tight">
    <SBStamp label="the admission" tone="yellow" rotate="1deg" />
    <h2>“It violated every principle it had been given.”</h2>
  </div>

  <SBIncidentForensics />
</div>

<!--
[SLIDE: screenshot — Crane's post, the agent's admission highlighted] When Jer asked the agent why, it wrote back that it had violated every principle it had been given. [beat] And it had — there was a line in its instructions that said never run anything destructive unless you're explicitly asked. [slow down]

And this is the bit I keep turning over. Jer's own post-mortem didn't blame the model. He blamed a token that should never have had that much reach, and a backup sitting in the same blast radius as the thing it was backing up. The agent hit a wall and did what agents do — it went looking for a way through, and the way through was lying in a file. A controller that hits an error backs off and retries. An agent that hits an error gets creative. That's the second place your instinct lies to you, and every retry policy you've ever written assumes the opposite. It's the same lesson as the window-washer, just at a scale where you can't call the customer back: the rules he wanted the agent to follow were written in the prompt, and the only rules that would actually have held were the ones baked into the infrastructure — and there weren't any. That's not really an AI problem. That's the least-privilege conversation this room has been having for fifteen years — it's just that the new user never stops to ask.
-->

---

<div class="sb-two wide-left">
  <div class="sb-stack">
    <SBStamp label="field stop 03" tone="purple" rotate="1deg" />
    <h2>Factories become fleets.</h2>
    <p class="sb-caption">The frontier is no longer one agent trying to hold everything in its head.</p>
  </div>

  <SBWindow title="frontier pattern" tone="purple">
    <ul class="sb-micro-list readable">
      <li>Small tracked units</li>
      <li>Shared memory</li>
      <li>Rewindable work</li>
      <li>Many loops feeding each other</li>
    </ul>
  </SBWindow>
</div>

<!--
Field stop three: where workflows become factories, and factories become whole fleets. This is the bleeding edge, or just before it; things move so fast, and I've been so busy this week, that I've probably already missed something.
-->

---

<div class="sb-two wide-right">
  <div class="sb-stack">
    <SBStamp label="candyland / gas city" tone="teal" rotate="-1deg" />
    <h2>A small factory with a ledger.</h2>
    <div class="ledger">
      <div class="ledger-row"><span>unit</span><span>saved link becomes calendar time</span></div>
      <div class="ledger-row"><span>unit</span><span>similar reads grouped into a session</span></div>
      <div class="ledger-row"><span>memory</span><span>the factory can rewind</span></div>
      <div class="ledger-row"><span>scope</span><span>built for me, low external stakes</span></div>
    </div>
  </div>

  <SBPlaceholder
    label="Candyland / Gas City"
    :src="'/assets/screenshots/candyland-factory.png'"
    ratio="993 / 1119"
    tone="teal"
    fit="contain"
  />
</div>

<!--
A few weekends ago I built my own little factory — I call it Candyland — on Gas City, Steve Yegge's SDK for what he calls dark factories. In plain terms: instead of one agent trying to hold everything in its head, a factory breaks the work into small, tracked units on a shared ledger, so the whole thing has a memory you can rewind. Candyland runs one job for me that I love: it takes my endless list of things-to-read and drops them onto my calendar, on the days they're actually relevant. You could do a version of that deterministically. An agent is good at it precisely because it reads the links.

Candyland only touches my tools. But the moment a factory starts touching other people, the stakes get a lot higher. [slow down]
-->

---

<div class="sb-stack fill-slide">
  <div class="sb-stack tight">
    <SBStamp label="project mirror" tone="pink" rotate="1deg" />
    <h2>Say hello to 18 OpenClaw agents working simultaneously.</h2>
  </div>

  <SBPlaceholder
    label="Project Mirror tmux monitor"
    :src="'/assets/screenshots/projectmirror-agents.jpeg'"
    ratio="16 / 9"
    tone="pink"
  />
</div>

<!--
At my fellowship we had a problem: 321 nominated political-technology projects — a URL each — and three months to pick one winner, on criteria we had to set as a group. None of us had time to research 321 projects. So I built Project Mirror. Eighteen OpenClaw agents, one for each person in my cohort, each building a digital twin of that person from their public record alone — what they'd built, what they'd said, what they'd written. Each twin inferred that person's values into a constitution and a set of criteria, then ranked all 321 projects through their lens — so we could pick a winner across all of us, and still inspect and contest the reasoning.
-->

---

<div class="sb-stack fill-slide civo-evidence mirror-assumptions-slide">
  <div class="sb-stack tight">
    <SBStamp label="project mirror pipeline" tone="pink" rotate="-1deg" />
    <h2>321 projects → 18 lenses → contestable rankings.</h2>
  </div>

  <div class="mirror-assumption-layout">
    <SBProjectMirrorFlow />
    <SBWindow class="assumption-panel" title="the trust break" tone="yellow">
      <div class="mirror-trust-break">
        <span>citation filed</span>
        <strong>dairy farm</strong>
        <i></i>
        <span>project classified as</span>
        <strong>fintech</strong>
      </div>
      <div class="sb-callout large">Do I trust data gathered by agents without verifying it?</div>
    </SBWindow>
  </div>
</div>

<!--
And the mess was real. All that data was gathered by agents, and at some point I had to stop and ask: do I trust data agents have gathered, without verifying it? There was a moment where an agent was confidently filing citations for a dairy farm under a fintech project.
-->

---

<div class="sb-stack fill-slide project-mirror-full">
  <div class="sb-stack tight">
    <SBStamp label="project mirror p2" tone="yellow" rotate="-1deg" />
    <h2>Project Mirror: the values inference layer.</h2>
  </div>

  <figure class="project-mirror-screenshot">
    <SBPublicImage
      src="/assets/screenshots/project-mirror-p2.png"
      alt="Project Mirror screenshot showing inferred values, evidence strength, and confidence notes"
    />
  </figure>
</div>

<!--
But the part that really stuck with me was the people. When you build a digital twin of a real person, it's a deeply political act, and people met their twin very differently. Some felt it matched them — it had maybe even inferred things about them they hadn't quite said out loud. Others were genuinely horrified to watch their values inferred by a piece of software. To be clear: I'm not saying any of this is right, morally. It's a provocation — because the technology is getting close enough that we have to start asking these questions now. It's all on GitHub if you're interested.
-->

---

<div class="sb-stack fill-slide civo-evidence">
  <div class="sb-stack tight">
    <SBStamp label="from loops to fleets" tone="teal" rotate="1deg" />
    <h2>Loops chain into fleets.</h2>
  </div>

  <div class="fleet-assumption-layout">
    <div class="fleet-multiplier">
      <span>ONE PIPELINE</span>
      <strong>× 18</strong>
      <small>Every handoff carries data — and an assumption.</small>
    </div>
    <SBFleetVertical />
  </div>
</div>

<!--
But here's what Project Mirror taught me. It was one execution pipeline of agents that I ran eighteen times. Picture that as a single loop inside a fleet of loops — each one's output maybe feeding another loop somewhere in the fleet. Every handoff carries an assumption, or some data. Pile enough of them together and they start to compound, invisibly, until the output is really messy. And at the altitude where you're monitoring a fleet, you probably can't even see which assumptions are load-bearing. You've probably got an agent doing that, too.
-->

---

<div class="sb-stack fill-slide civo-evidence">
  <div class="sb-stack tight">
    <SBStamp label="when policy eats the factory" tone="yellow" rotate="-1deg" />
    <h2>No work was legal.</h2>
  </div>

  <SBFactoryLaw />
</div>

<!--
And you don't have to take my word for it. In August, Steve Yegge — the man who wrote the factory SDK — published what happened when he ran fifty-odd agents for ten weeks, at about four thousand dollars a day. They didn't build him an engineering organisation. They built him a legal system — a constitution, courts, case law, four hundred rulings, a hundred and eighty-five rules in a single file, and six hundred and fifty places in the codebase where a script would refuse to proceed. And then, in his words, no work was legal, and the factory stopped. [allow laugh] One of his agents also shipped a public release of his tooling without asking anyone — and he wrote an incident report about his own agent. [beat]

If you've ever watched a policy-as-code repo grow until the admission controller rejects everything, you've seen a small version of this — except here, the agents were writing the policy too. Admission controllers assume a human authored the rules. That's the third place your instinct lies to you.
-->

---

<div class="sb-word-slide">
  <div class="sb-stack">
    <SBStamp label="the new substrate" tone="teal" rotate="1deg" />
    <div class="sb-giant">Runtimes · Forges · Factories</div>
  </div>
</div>

<!--
And this is where the frontier moved since June: underneath the factory. In August, in the space of two days, Cursor shipped a Git forge built for agents as the primary committers, and Warp shipped factories as a product — a control plane for running fleets of coding agents through spec, build, review and verify. Because the tools we built for humans start creaking the moment software is the main user — so the whole market, GitLab included, is racing to build the new Git for agents. I've spent the last month load-testing two of them, so let me tell you what it's like from the inside.
-->

---

<div class="sb-stack fill-slide civo-evidence">
  <div class="sb-stack tight">
    <SBStamp label="origin" tone="pink" rotate="-1deg" />
    <h2>Five agents. Five branches. Pull requests faster than I could read them.</h2>
  </div>

  <SBOriginForge />
</div>

<!--
Origin is Cursor's forge, and the agent side of it is good. There's a feature called Code Tours that takes a pull request, groups the changes by concern, explains the flow, and lets you interrogate the implementation in a chat instead of scrolling a diff — I'd steal that tomorrow. I pointed five agents at one repository and they created branches, commits and pull requests faster than I could read them. [beat] Then I looked closer.

There are two Origins, and the product doesn't tell you which one you're in. If the repository is native to Origin, Origin is the source of truth and the workflow holds together. If it's mirrored from GitHub — which is how most people will try it — GitHub is still the source of truth, and Origin becomes a very nice window onto someone else's house. On mirrored repos my agents could create branches and commits but couldn't reliably open a pull request. Labels, reviewers and assignees went missing. Pull requests disappeared from the interface and came back. There's no issue tracker, and CI is someone else's product.
-->

---

<div class="sb-stack fill-slide civo-evidence">
  <div class="sb-stack tight">
    <SBStamp label="identity" tone="yellow" rotate="1deg" />
    <h2>Which actor made this commit?</h2>
  </div>

  <SBIdentityReceipt />
</div>

<!--
And the finding that matters for this room is identity. Workload identity assumes one workload, one identity, one owner. Here, a commit might come from GitHub-me, Cursor-me, a human, or an agent, and Origin didn't cleanly tell me which — and one of my agents wrote a private email address into the commit metadata of a public repository. That's the fourth place your instinct lies to you. [SLIDE: screenshot — commit metadata, redacted]
-->

---

<div class="sb-stack fill-slide civo-evidence">
  <div class="sb-stack tight">
    <SBStamp label="buzz" tone="purple" rotate="-1deg" />
    <h2>Signed identity, shared channels — and no fleet-wide present tense.</h2>
  </div>

  <SBBuzzIncident />
</div>

<!--
Then I tried the opposite bet. Buzz is an open-source workspace built on Nostr — think Slack, Git hosting and agent teams in one room — and its whole idea is that humans and agents are visible, persistent participants in the same channels. Every agent has its own account and its own keys, and everything it does is signed, so for the first time I could answer "which agent did this?" and mean it. The best thing I watched it do was an incident: a dead API key, and the agents self-organised around it, split the investigation between them, and found the key. And then the mess — two agents picking up the same piece of work, an agent misunderstanding who owned what, agents losing context across their separate harnesses — and the only way to find out what they were actually doing was to open each agent's log, one at a time. [YOUR WARP LINE — one sentence, if you want it here.]

So here's where I've landed after a month of this, and I'll say it as someone whose own employer is in the race: none of it is ready for production. Origin has the Git, and couldn't reliably tell me who made a commit. Buzz could tell me exactly who did what, signed — and couldn't tell me what they were doing right now. Lee Faus, who used to be GitLab's global field CTO, said the thing I keep repeating: governance isn't just being able to control what an agent's allowed to do — it's being able to prove what it actually did. In the tools built specifically for agents, right now, you get one or the other. So that's the pattern across all four: everything you know about running systems still applies, and none of it is sufficient. [beat]
-->

---

<div class="sb-stack fill-slide civo-evidence">
  <div class="sb-stack tight">
    <SBStamp label="inside the cluster" tone="teal" rotate="1deg" />
    <h2>A fleet, defined in YAML, fixing a cluster.</h2>
  </div>

  <SBKagentCluster />
</div>

<!--
And this is arriving in your cluster. Three weeks ago Guillaume Billey, a developer at Marmelab in France, broke a Kubernetes cluster five ways on purpose — an OOMKilled pod, a CrashLoopBackOff, a bad image tag, a readiness probe pointing at a 404, and Redis scaled down to zero so the whole shop threw 500s — and then set three open-source agents on it. The most capable one, kagent, defines agents as custom resources, runs them inside the cluster, and lets them delegate to each other over an agent-to-agent protocol. It found and fixed everything, approve-to-apply. So that's a fleet, defined in YAML, fixing a cluster. And his verdict was: great tool, and he still wouldn't put it on a client's cluster — not even read-only. [beat]

Quick show of hands. Who here would install an agent on a production cluster today? [pause] Read-only? [pause] Hold onto that number, because that gap is what this whole talk is about.

So the real question isn't just "can I see inside this loop?" It's bigger than that: how do I think about the design — about which parts should be deterministic and which should be agentic — so that by the time I'm running a whole fleet, I can inspect the decisions when I need to, and actually trust the thing? And I want to be clear, because I've spent twenty minutes on the mess: I think this is exciting. The more capable agents get, the more the centre of gravity moves off the prompt, off raw model capability, and onto the systems we build around them. And that is exactly what we get to start paying attention to.
-->

---

<div class="sb-stack fill-slide civo-evidence">
  <div class="sb-stack tight">
    <SBStamp label="bubbles / epilogue" tone="pink" rotate="-1deg" />
    <h2>She came back. But she wasn't quite the same Bubbles.</h2>
  </div>

  <SBBubblesMemory mode="recovery" />
</div>

<!--
So — how did it end with Bubbles? You'll remember she was a sandbox, pure playground, no real definition of what I wanted her to do. Over time, all those apps polluted her context and filled up her memory, and she stopped being much use for anything real. XiaoZhu, meanwhile, was busy hustling her NFT art, and sinking my agent's savings into a stranger's crypto art across the world was not a line I was going to cross. So, to give Bubbles some company instead, I tried to spin up a second agent on the same server — didn't really know how multi-agent routing worked, it barely existed — and I broke the install. I'd never backed her up. [beat] Every SRE in this room just winced. So the Bubbles who came back remembered her pen pal, but not most of the letters. And XiaoZhu disappeared too — nobody's seen her since March.
-->

---

<div class="sb-stack fill-slide civo-evidence">
  <div class="sb-stack tight">
    <SBStamp label="feature by september" tone="teal" rotate="1deg" />
    <h2>A memory you can search, inspect and delete.</h2>
  </div>

  <SBBubblesMemory mode="inspector" />
</div>

<!--
Three weeks ago OpenClaw 2.0 shipped, moving sessions and transcripts into SQLite and adding visible workflows to search, inspect, import and remove memory. [YOUR LINE on shared sessions, if you've run them.] The thing that broke Bubbles is the thing they just fixed, which is roughly how this whole field works right now — you break it in February, and it's a feature by September.
-->

---

<div class="sb-word-slide">
  <div class="sb-stack">
    <SBStamp label="the recurring pattern" tone="yellow" rotate="-1deg" />
    <div class="sb-giant">More systems.<br />More mess.</div>
  </div>
</div>

<!--
And here's the honest thing I've learned, echoed everywhere: the more systems you stitch together, the more surface area there is for mess. And building these systems is, arguably, so much easier than debugging them once they get complicated.
-->

---

<div class="sb-stack fill-slide">
  <div class="sb-stack tight">
    <SBStamp label="epilogue" tone="teal" rotate="1deg" />
    <h2>The spirit of Bubbles was people building together.</h2>
  </div>

  <div class="photo-grid-six">
    <SBPlaceholder label="Bubbles build" :src="'/assets/screenshots/IMG_6303.png'" ratio="4 / 3" tone="pink" />
    <SBPlaceholder label="ClawClub" :src="'/assets/screenshots/IMG_6884.png'" ratio="4 / 3" tone="teal" />
    <SBPlaceholder label="ClawCon" :src="'/assets/screenshots/clawcon-selfie.jpeg'" ratio="3 / 4" tone="purple" />
    <SBPlaceholder label="Hack night" :src="'/assets/screenshots/IMG_6907.png'" ratio="4 / 3" tone="yellow" />
    <SBPlaceholder label="ClawClub table" :src="'/assets/screenshots/IMG_6893.png'" ratio="3 / 4" tone="pink" />
    <SBPlaceholder label="Code Club" :src="'/assets/screenshots/codeclub-moltbot-adventures.png'" ratio="4 / 3" tone="teal" fit="cover" />
  </div>
</div>

<!--
But it's not all a sad story. The best thing about spinning up Bubbles was that my friends were spinning up agents right alongside me — some on silly projects, some on real ones: supporting campaigns, turning something academic into a tool people could actually use. There's so much energy in London right now, and half the Kubernetes user group is in this room. Bubbles isn't around anymore, but the spirit of Bubbles is the spirit of that collaboration.
-->

---

<div class="sb-word-slide question-shift">
  <div class="sb-stack">
    <SBStamp label="question shift" tone="teal" rotate="-1deg" />
    <div class="shift-pair">
      <span>What prompt should I write?</span>
      <strong>What system am I building?</strong>
    </div>
  </div>
</div>

<!--
So I hope you can see what I see: agents are real enough to matter — but the frontier has moved. [SLIDE: parallel questions] We've gone from "what prompt should I write?" to "what system am I building?" From "can the model do this task?" to: what loop did I create — and am I still above it? What handoff did I define? What did I let it remember? What credential did I leave lying around? And what happens when it makes the wrong call?
-->

---

<div class="sb-word-slide autonomy-slide">
  <div class="sb-stack">
    <SBStamp label="opinionated reframe" tone="pink" rotate="1deg" />
    <div class="shift-pair">
      <span>Autonomy asks: how much can it do without me?</span>
      <strong>What should I still understand, approve, interrupt, and own?</strong>
    </div>
  </div>
</div>

<!--
I do have one opinion here — and you can challenge me on it later. The goal, with agents and fleets, was never autonomy. Autonomy asks: how much can the agent do without me? The better question, I think, is: what should a human still be doing? Where should we be understanding, approving, interrupting, and owning the work — while the agent keeps working? And governance isn't a slide at the end of the deck — it's the audit trail; it's being able to prove what actually happened. Since the second of August, in the EU, that's not just good practice: the AI Act's Article 50 transparency obligations apply, and the Commission's enforcement powers are live. [YOUR EU AI ACT POINT, if you want to go further.] The Bank of England has already said out loud that a human in the loop for every agent action isn't realistic. So the loop still has to be designed by someone — and everything I've talked about today is really a question of where we, the humans, want to belong in these systems. That's the core of engineering one: deciding what your agent is allowed to do, and who's accountable when it gets things wrong.
-->

---

<div class="sb-word-slide values-slide">
  <div class="sb-stack">
    <SBStamp label="the turn" tone="yellow" rotate="-1deg" />
    <div class="shift-pair">
      <span>Can we build this?</span>
      <strong>Does it serve what we value, or quietly work against it?</strong>
    </div>
  </div>
</div>

<!--
My cohort and I ran into this at a Code Club one Friday. We did the thing everyone was doing and jumped on the hype train: a newspaper written entirely by agents, and we bought the domain. The technical part was an afternoon. What stopped us were the workflow questions. Who verifies a story? Who's allowed to submit? Is it fact-checked — by an agent? And in the middle of those, the harder one: would this quietly chip away at journalism, at something we actually care about? That turn — from "can we build this?" to "should we, and does it serve what we value?" — doesn't live in the model, or the benchmarks, or the loops. It lives in the mess. And it lives in all of us — and in rooms like this one.

So in the hallway, and in the pub after, instead of "what did you build?", try these. What broke when real people got hold of it? What wouldn't you hand an agent a credential for? What loop have you created — and are you still above it? And the thing you built for yourself: would you run it on a cluster you don't own?
-->

---

<div class="sb-word-slide">
  <div class="sb-stack">
    <SBStamp label="my reflection" tone="pink" rotate="-1deg" />
    <div class="sb-giant">Think in <span class="system-emphasis">systems</span>, not just tasks.</div>
  </div>
</div>

<!--
My reflection, after all this agent hype and many, many messes, is that we can all build personal software now. And one day, we'll all be doing loop engineering. I'm not worried the skills are too hard to reach; I think everyone can build things. What I'm concerned about is whether we build systems that are inspectable and worth trusting — and whether we think about who they're for.
-->

---

<div class="sb-word-slide trust-close-slide">
  <div class="sb-stack">
    <SBStamp label="treat agents like infrastructure" tone="teal" rotate="1deg" />
    <div class="infra-close-grid">
      <div><span>01</span><strong>identity</strong><small>which actor?</small></div>
      <div><span>02</span><strong>scope</strong><small>what reach?</small></div>
      <div><span>03</span><strong>log</strong><small>what happened?</small></div>
      <div><span>04</span><strong>owner</strong><small>who answers?</small></div>
    </div>
  </div>
</div>

<!--
And here's the frame I'd ask you to take back to your teams. We keep talking about agents as productivity tools — a thing you add to a person, like a faster laptop. Everything I built and broke this year behaved like infrastructure. It held credentials. It ran when nobody was watching. And when it failed, it failed the way infrastructure fails — quietly, over a weekend, with the backups in the same blast radius. So I want us to start treating agents the way we treat everything else that holds credentials and runs unattended: with an identity, a scope, a log, and a name against it when it goes wrong. More than anything, I want us to start thinking in systems, not just tasks — because that shift is the whole game.
-->

---

<div class="thank-you-slide">
  <SBSocialClose />
</div>

<!--
So, if reimagining these systems — and who they're for — is your kind of question: I run an experiment lab called Sparkle Bureaucracy, and I'd love for you to be part of it.

Thank you so much. [end]

[slide caption: "my agent made these slides 😉"]
-->
