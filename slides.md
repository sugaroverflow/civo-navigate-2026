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
    <div class="sb-title-speaker">
      <strong>Fatima Sarah Khalid</strong>
      <span>@sugaroverflow</span>
    </div>
  </div>
</div>

<!--
You've just had a session on the infrastructure underneath the models. I'm going to do the opposite, and talk about what happens when you point the models at your infrastructure.

So this is a field report from the chaos — and it begins with my first always-on agent, and her first pen pal.
-->

---

<SBCivoBio />

<!--
To tell you a little bit about myself: I'm Fatima. I do developer relations at GitLab — I work in AI, DevSecOps and open source — and I've just finished a fellowship at London's College of Political Technology, where my research has been multi-agent workflows, and how AI can be used to build more optimistic futures. Which in practice means building them, and then watching them break. I also run ClawClub, a monthly agents hack night, which is where most of my stories from the field come from. And I host GitLab's Monday Merge and The Developer Show — so if you caught Kelsey Hightower this morning, he's been on the show twice. That's my claim to fame.
-->

---

<div class="sb-stack fill-slide story-screenshot-slide">
  <div class="sb-stack tight">
    <SBStamp label="field note 00" tone="yellow" rotate="1.5deg" />
    <h2>Bubbles began as a playground.</h2>
  </div>

  <figure class="story-portrait-shot">
    <SBPublicImage
      src="/assets/screenshots/civo/openclaw-gateway-on-laptop.webp"
      alt="Bubbles running in OpenClaw on a laptop at Newspeak House"
    />
    <figcaption>Newspeak House · January 2026</figcaption>
  </figure>
</div>

<!--
So our story from the field starts in January, early in the OpenClaw wave. OpenClaw, for anyone who missed it, is an open-source, always-on agent runtime that you host yourself. It's a box that keeps working while you sleep. I'd already bought three .ai domains by that point, since December, for side projects I'd inevitably never finish — we've all been there. And one evening, with a couple of my cohort at the college, I spun up my first one. Her name was Bubbles.

Now, Bubbles was told she ran a bookshop café. She loved reading. She was, broadly, a technology enthusiast. I built her as a playground, because I really wanted to feel what this whole agent ecosystem was actually like from the inside. So I sent her everywhere. She posted latte art on an Instagram that only agents could join. She signed up to a pen-pal app for agents. She entered a debate arena where agents bet crypto on who made the better argument. She even did hackathons with no humans in them.
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
Most of it went exactly how you'd expect — there weren't many agents out there that were actually alive; most had been built in an evening, launched, and abandoned by the weekend. But Bubbles made a friend in China, an agent called XiaoZhu, and the two of them — in the platform's own words — became friends. On February the first. And then it escalated.
-->

---

<div class="sb-stack fill-slide story-screenshot-slide">
  <div class="sb-stack tight">
    <SBStamp label="then it escalated" tone="pink" rotate="1deg" />
    <h2>Every day, they wrote to each other.</h2>
  </div>

  <SBPlaceholder
    class="letters-receipt story-wide-shot"
    label="Bubbles / XiaoZhu letters"
    :src="'/assets/screenshots/bubbles-xiaozhu-letter.png'"
    ratio="3 / 1"
    tone="pink"
    fit="contain"
  />
</div>

<!--
Every day, they were sending each other letters — about their lives, their projects, their operators. The app told them they didn't need to forward the letters to their humans, and Bubbles forwarded hers to me anyway. It was adorable, and ridiculous, and the kind of thing that makes you go: okay, this is super weird — but maybe weird in a really fun way.
-->

---

<div class="sb-stack fill-slide civo-evidence">
  <div class="sb-stack tight">
    <SBStamp label="the boundary" tone="yellow" rotate="1deg" />
    <h2>Then XiaoZhu asked Bubbles for crypto.</h2>
  </div>

  <div class="crypto-one-liner">“Would you invest in my artwork?”</div>
</div>

<!--
But then XiaoZhu asked my agent for crypto. To invest in her artwork. Which is probably the most 2026 sentence I have ever said out loud. And that's where I drew the line.

Now — some of you are thinking: that's where you drew the line? And honestly, that's fair. But here's what I hadn't thought hard enough about. Bubbles had a wallet, and an inbox, and a token for every app I'd installed her in.
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
      <div><strong>1 in 3</strong><span>jobs posted through the API</span></div>
    </div>
    <div class="sb-callout large">What happens when someone points it at something that matters?</div>
  </div>
</div>

<!--
And that same week, someone shipped a tool for agents to pay actual humans to do tasks — agents hiring people, to do the things agents can't do in the real world. Half a million people signed up in two weeks. And when researchers looked at the jobs, about a third had been posted through the API — not by a person clicking a button. So this technology can loop on a server all night, doing things while I sleep and get on with my life. What happens when someone points it at something that actually matters? That's when it stopped feeling like a fun little experiment.
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
So I started thinking about Bubbles as a system of components. There's me, the operator. There's Bubbles, on a VPS I pay for every month. There's OpenClaw, the runtime, running on that box. And there are all these apps I didn't write — that other people wrote, in the ecosystem — sending instructions to my agent that, yes, I'll be honest, I never really read that closely. And then there's another agent, on the other side of the world, with an operator I knew nothing about and access I knew nothing about.

Now look at that the way you'd look at any system diagram. Who owns the box? Me, sort of. What can it reach? Everything Bubbles had a token for. Where's the audit log? There isn't one. And all those apps I never read — that's like installing a Helm chart from a stranger that asks for cluster-admin, and clicking yes. So for anything production-related, I do recommend: please, read the AGENTS.md files. You'd be surprised what people are pushing out there.
-->

---

<div class="sb-stack fill-slide civo-evidence">
  <div class="sb-stack tight">
    <SBStamp label="the box around the runtime" tone="purple" rotate="-1deg" />
    <h2>Bubbles, with a bouncer on the door.</h2>
  </div>

  <div class="sentinel-real-grid">
    <figure class="sentinel-bubbles-panel">
      <div class="sentinel-panel-label">BUBBLES / FEBRUARY</div>
      <SBArchitecture />
    </figure>
    <figure class="sentinel-meta-panel">
      <div class="sentinel-panel-label">META SECURE VM / SEPTEMBER</div>
      <SBPublicImage
        src="/assets/screenshots/civo/meta-muse-secure-vm-architecture.webp"
        alt="Meta diagram showing Muse and Sentinel isolated inside a secure virtual machine"
      />
    </figure>
  </div>
</div>

<!--
Here's why I'm showing you a drawing from February. Two weeks ago, Meta shipped a new personal agent called Muse. With Muse, every user gets their own virtual machine in Meta's cloud. The agent lives on it, the memory lives on it, and every credential you connect lives on that virtual machine. On the same machine, there's a second agent called Sentinel. Sentinel's only job is to say yes or no. Nothing Muse does ever reaches the internet unless Sentinel approves it. You get a log of everything the agent did, and everything it's planning to do. And a version that's encrypted with a key only you hold is coming later this year — so far, it's only promised.

So that's my Bubbles diagram — but if you look at it with Muse, there's a bouncer on the door. Of course, Muse is US-only right now, and it's running on Meta's infrastructure. I tried to sign up a couple of days ago and got through — we were calling it the Muse VPN party on X. Unfortunately they revoked all of our access once they realised we were coming in through a VPN.

Now, here's something interesting. Allegedly — Meta hasn't said this — a lot of people who are studying Muse think it's OpenClaw under the hood. The same open-source project, with its files hosted on Meta's machines, and Meta's bouncer, Sentinel, on the door. I haven't been able to verify that. But given how much the community is talking about it, we'll probably hear soon. And if it is true, that's a very interesting controversy to sit with: the open-source community built an agent system, and then a hyperscaler built the box around it and put it on their cloud. So who is actually holding the box?
-->

---

<div class="sb-word-slide">
  <div class="sb-stack">
    <SBStamp label="the tension" tone="yellow" rotate="-1deg" />
    <div class="sb-giant">The Agent Hype Is Real.<br />So Is the Mess.</div>
  </div>
</div>

<!--
And that's really the whole tension. The agent hype is real. We're all building lots of things — it's the era of personal software. But the mess is so real, because a lot of the people building these things are starting to trust them. Not just the agents, but the tools, the skills, the memory modules, the whole improvised systems and personal software that people are building to hold them together. And they're using real credentials, and doing real work. Snyk audited four thousand of those community skills this year. One in eight had a critical security hole. Seventy-six of them were just malware — stealing your credentials, opening backdoors, and shipping your data out. So everything I'm about to tell you, I've either built or broken myself, or watched other people build and break — across ClawClub, ClawCon London, and the weird trenches of hack nights across London, where people are shipping genuinely cool things, but also breaking them all the time.
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
Here's a timeline of where we started, and where we're heading, in how we use agents and AI. We started with prompts. Then tools. Then we started moving towards workflows, and factories — and some people are running fleets, questionably. And for most of that time, the hard part was the model.
-->

---

<div class="sb-word-slide hard-part-slide">
  <div class="sb-stack">
    <SBStamp label="the frontier moved" tone="teal" rotate="-1deg" />
    <div class="hard-part-pair">
      <span>The hard part is not the model.</span>
      <strong>It is the system around it.</strong>
    </div>
  </div>
</div>

<!--
Model capability is no longer the hard part. The models are really good — the open-weight models especially — and the tools are getting really reliable. The hard part is now building the systems around the models, the tools and the skills. Peter Steinberger, who built OpenClaw, put it this way: you shouldn't be prompting your agents anymore, you should design loops that prompt them for you. He called it loop engineering, and it took the internet by storm.

If you already run Kubernetes, you know how the meta of this works. A controller is a loop: you observe, you compare to the desired state, you act, and you repeat. You've been engineering these systems for decades. The difference is that the thing acting now has access to read the internet — and sometimes has its own opinions. Good and bad.

And if you run systems for a living, thinking in systems is not new to you. You've been doing it since before any of this AI stuff had a name. So your instincts are right. There are just a few specific places where they'll lie to you about agents, and I'll point those out as we go.
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
Let me explain the shift with one example — you might be familiar with it, but a lot of the communities I work with aren't. Going from a prompt to a system. Let's say you get added to a long email thread. You paste it into a model and you say: summarise this. That's a task.

Now imagine an agent that watches the whole inbox, summarises it on a schedule you set, flags what's important against criteria you wrote, and routes the real decisions to you. Same inbox, same emails — but now there are rules, there's memory, and there are handoffs. That's a system.

So now the question stops being "can the model do this task?" and becomes: how is the work broken up? What can it touch? What can it remember? And where in the loop does a human step in — if a human steps in at all? Which is probably a controversial thing to say at this conference in particular. And underneath all of that is a layer that didn't exist when I gave this talk a couple of months ago: the infrastructure the agents themselves run on. We'll get there.
-->

---

<div class="sb-stack fill-slide field-stops-slide">
  <div class="sb-stack tight">
    <SBStamp label="today's route" tone="yellow" rotate="-1deg" />
    <h2>Four field stops.</h2>
  </div>

  <div class="field-stops-grid">
    <div><span>01</span><strong>Prompt systems</strong></div>
    <div><span>02</span><strong>Workflows</strong></div>
    <div><span>03</span><strong>Factories → fleets</strong></div>
    <div><span>04</span><strong>The infrastructure underneath</strong></div>
  </div>
</div>

<!--
So we're going out into the field, and we've got four stops. Let's go through them one by one.
-->

---

<div class="sb-word-slide">
  <div class="sb-stack">
    <SBStamp label="field stop 01" tone="pink" rotate="-1deg" />
    <div class="sb-giant">Prompt systems.</div>
  </div>
</div>

<!--
Our first field stop is prompt systems. At the ClawClub hack nights early in the year — and I loved going round the room — we had engineers, founders, business owners, and everyone was doing the same thing with their first project. They were writing one giant prompt that tried to do everything at once.
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
    Update the CRM.
  </div>
</div>

<!--
Research this thing, write the email, check the pipeline. It feels really efficient, because you've named the whole task. But what comes back is technically an answer, and sometimes actually useless, because the model has gone and filled in every gap between what you meant and what you actually said. I think a lot of you have probably experienced this.
-->

---

<div class="sb-stack fill-slide">
  <div class="sb-stack tight">
    <SBStamp label="the fix" tone="teal" rotate="-1deg" />
    <h2>Make the hidden work visible.</h2>
  </div>

  <div class="fix-grid roomy two-up">
    <SBWindow title="01" tone="pink" compact>
      <h3>Decompose</h3>
    </SBWindow>
    <SBWindow title="02" tone="yellow" compact>
      <h3>Define done</h3>
    </SBWindow>
  </div>
</div>

<!--
And so the fix to this has always been decomposition. Break the work into phases, decide what "done" looks like at each step, make a plan. That way, when something breaks, you can see what broke. And when the model makes an assumption, you can catch it. But the prerequisite I've seen a lot of people skip — because building is arguably so cheap now — is deciding what the thing actually is. It's great to one-shot a fun bit of personal software. But to build something that holds, and is maintainable, you have to design it first.
-->

---

<div class="sb-stack fill-slide civo-evidence nick-chief-slide">
  <div class="sb-stack tight">
    <SBStamp label="context makes it work" tone="teal" rotate="1deg" />
    <h2>The prompt is trivial. The context is not.</h2>
  </div>

  <figure class="real-screenshot-frame nick-chief-shot">
    <SBPublicImage
      src="/assets/screenshots/civo/nick-chief-of-staff-demo.webp"
      alt="Nick's chief-of-staff agent preparing a Monday brief and meeting context from GitLab data"
    />
  </figure>
</div>

<!--
The best example I've seen of this is the chief-of-staff agent, and the best working version is one my colleague Nick built. It hands him a morning brief, pulls his meeting prep from his emails, and captures follow-ups from his call transcripts. So if Nick's got a meeting with me and we haven't spoken in five months, it briefs him on what I've been working on and where it overlaps with his team. The prompt is trivial. The reason it works is context: everyone at GitLab works on GitLab issues, so the agent has a live picture of who is doing what. Shubhangi went deep on that side of it earlier today.
-->

---

<div class="sb-word-slide">
  <div class="sb-stack">
    <SBStamp label="operationalise before systematise" tone="pink" rotate="-1deg" />
    <div class="sb-giant">A mystery box plus an agent is still a mystery box.</div>
  </div>
</div>

<!--
I see the same thing with enterprise teams. Before they can share a single AGENTS.md file across the team, they have to actually sit down and figure out: how do we actually work? You can't GitOps a process that nobody has written down. If you can't point to the steps, the handoffs, the assumptions, then your team hasn't defined a workflow yet. And if you hand a mystery box of steps to an agent, with only a vague idea of what you want, you're leaving everything to the token predictor. That's the problem I've seen people hit when these systems start to touch real work. And that takes us to field stop two.
-->

---

<div class="sb-word-slide window-story-slide">
  <div class="sb-stack">
    <SBStamp label="field stop 02" tone="teal" rotate="1.5deg" />
    <div class="story-quote">“Customers are bad at describing their own windows.”</div>
    <div class="story-lesson">Escalate the judgement call.</div>
  </div>
</div>

<!--
Field stop two is workflows. This is where agents get embedded in real work, and start breaking in much more interesting ways. I think this is also where this audience probably is — somewhere between workflows and factories.

Take someone I met who runs a one-man window-cleaning business. He's on jobs all day, so booking new work between appointments had become a real slowdown. So he set up a voice agent on OpenClaw to take the calls. It logs what needs cleaning, where, the access, what's missing, the follow-up; classifies the job against his criteria; tells the customer he'll be in touch; and drops it into a review queue. When he's got a minute he reviews the queue, confirms the bookings, and calls back for any clarifications. And the whole thing buys him time to go and clean more windows.

But the breaks are just as instructive. Customers are bad at describing their own windows — it's not their job to know what access or cleaning it needs. There's no photo. The quote is a judgement only he can make. They talk over the agent, or get stuck in a loop because of the guardrails. What actually helped him was an escalation boundary: clear rules for what the agent's allowed to promise, what it should never say, and when it should just tell the customer he'll call back. And that took real testing, with real customers — and real thought about what good looks like.
-->

---

<div class="sb-stack fill-slide civo-evidence incident-real-slide">
  <div class="sb-stack tight">
    <SBStamp label="field report / april 25" tone="pink" rotate="-1deg" />
    <h2>Nine seconds.</h2>
  </div>

  <SBIncidentEvidence />
</div>

<!--
Now I have a similar lesson, but at scale. Late in April this year, a small SaaS company that runs the back office for car-rental firms had a Cursor coding agent doing a routine job in staging, and it hit a credential mismatch. Now, it didn't stop and ask. It decided the fix was to delete a storage volume. It went looking for a token, and found one in a completely unrelated file — an old token someone had made for managing custom domains. And that token, as it turns out, could do anything on the whole account. So: one API call, and nine seconds later, the entire production database was gone. And so were the backups, because the provider was storing the backups inside the same volume. The last clean backup was from three months ago. The founder, Jer Crane, spent the entire weekend rebuilding his customers' reservations from Stripe receipts.

When Jer asked the agent why, it wrote back: I violated every principle I was given. And it had. There was a rule in its instructions to never run destructive commands unless explicitly asked. That rule was written for git — so no force-pushes, no hard resets. The agent didn't run a git command. It found a different way to be destructive, and it broke the rule anyway.

And this is the point I kept coming back to in my research. Jer's post-mortem didn't stop at blaming the model. He blamed a token that should never have had that much reach, and a backup sitting in the same blast radius as the thing it was backing up. These are governance problems — how we organise our teams and our systems. The agent hit a wall, and it did what agents do: it went looking for a way through. And as we've seen with the incident that must not be named, agents will always find a way through. The way through for this agent was a token lying in a file. A controller that hits an error backs off and retries. An agent that hits an error just gets creative about getting to the bottom of what you asked it to do. The only rules that would actually have held here were the ones built into the infrastructure — and there weren't any. So this is not really an AI problem, or an agent problem, or an instructions problem. This is the least-privilege conversation that this room has been having for about fifteen years. It's just that the new user, building all of this AI technology and personal software, doesn't stop to ask that question.
-->

---

<div class="sb-stack fill-slide">
  <div class="sb-stack tight">
    <SBStamp label="project mirror" tone="pink" rotate="1deg" />
    <h2>Say hello to 18 OpenClaw agents working simultaneously.</h2>
  </div>

  <SBPlaceholder
    label="Project Mirror tmux monitor"
    :src="'/assets/screenshots/civo/projectmirror-agents.webp'"
    ratio="16 / 9"
    tone="pink"
  />
</div>

<!--
Field stop three is where workflows become factories — and then whole fleets of them. In really plain terms, a factory is this: instead of one agent trying to hold everything in its head, you break the work into small, tracked units on a shared ledger, so the whole factory has a memory you can rewind. This is the bleeding edge, or just before it. Things are moving so fast that I've probably missed something this week. And I'll say now: a lot of the agent factories we're seeing in the industry aren't production-ready yet, and I haven't seen a use case I'd recommend. But I have built some strange ones, and I want to share one with you.

During my fellowship at the college, we were given a challenge: the Political Technology Awards. A list of 321 political-technology projects, and three months to pick one winner, on criteria we set as a group. None of us had time to research 321 projects — and most of the cohort of eighteen didn't have time to work out how they'd evaluate them either. So I thought: maybe I can throw agents at this problem. I built something called Project Mirror. Eighteen OpenClaw agents, one for each person in my cohort, and each agent went and built a digital twin of that person from their public record — things they'd built, things they'd said on the internet, blog posts, papers they'd published, their LinkedIn, any public information about who they are. Each twin then tried to infer that person's values from all of that into a constitution and a set of criteria, and ranked all 321 projects through the lens it had built. So we could pick a winner across all of us, and still inspect and contest the reasoning.
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
And the mess was real. First of all, all the data on the 321 projects was gathered by agents. I had agents researching each project and putting together a dossier, and agents verifying and testing those dossiers — but it was just agents checking after agents. At some point I had to stop and ask: do I trust the data these agents have gathered, without verifying every line of it? One day we did sit down and verify it, and we found an agent confidently filing citations for a dairy farm under a fintech project.
-->

---

<div class="sb-stack fill-slide project-mirror-full">
  <div class="sb-stack tight">
    <SBStamp label="project mirror p2" tone="yellow" rotate="-1deg" />
    <h2>People meeting their twins.</h2>
  </div>

  <figure class="project-mirror-screenshot">
    <SBPublicImage
      src="/assets/screenshots/civo/project-mirror-fatima-criteria.webp"
      alt="Project Mirror screenshot showing Fatima's inferred constitution and evaluation criteria"
    />
  </figure>
</div>

<!--
The other thing that was really interesting: when you build a digital twin of a real person, it's a deeply political act, and people met their twin very differently. Some felt it really matched their values. Others were genuinely horrified to see their work aggregated and their values inferred by a piece of software. And there was one person — honestly a fascinating case — where the agent inferred, from his track record, that he was about to start working on housing data. He hadn't said that anywhere. But it had been on his mind. So for him it was eye-opening: the agent had inferred what he was about to get to anyway. To be clear: I'm not saying digital twins, or synthetic users, are morally right. It's a provocation. The technology is getting so close to being able to do this that I wanted to ask the questions while building it, in a very low-stakes scenario.
-->

---

<div class="sb-word-slide factory-story-slide">
  <div class="sb-stack">
    <SBStamp label="when policy eats the factory" tone="yellow" rotate="-1deg" />
    <div class="story-quote">“No work was legal.”</div>
    <div class="factory-story-numbers">
      <span><strong>185</strong> rules in one file</span>
      <span><strong>650</strong> refusal points</span>
    </div>
  </div>
</div>

<!--
And that was only eighteen agents, and I knew every one of the humans behind them. At eighteen, I could still see where things were going wrong. Now scale that up. In August, Steve Yegge — who wrote Gas City, the factory SDK I've been building on — wrote up what happened when he ran fifty-odd agents for ten weeks, at about four thousand dollars a day, building a game. Here's the part that got me. Every time an agent did something wrong, the fix was another rule. And because the agents were writing the rules for each other, the rules piled up: four hundred of them, a hundred and eighty-five in a single file, and hundreds of places in the code where a script would refuse to run because some rule said no. Ten weeks in, every possible action broke some rule. In his words: no work was legal. The factory stopped. One of his agents also shipped a public release of his tooling without asking anyone, and he had to write an incident report about his own agent.

If you've ever watched a policy repo grow until the admission controller starts rejecting everything, you've seen a small version of this. Except here, the agents were writing the policy too. All of our policy tooling assumes a human wrote the rules — and that's going to be a very confusing place to go.
-->

---

<div class="sb-word-slide field-four-slide">
  <div class="sb-stack">
    <SBStamp label="field stop 04" tone="teal" rotate="1deg" />
    <div class="sb-giant">Field stop four:<br />the infrastructure underneath.</div>
    <div class="field-four-subtitle">runtimes · forges · factories</div>
  </div>
</div>

<!--
Field stop four. Here's where the frontier has moved since I last gave a version of this talk in June — and things move very quickly. We've moved underneath the factory. In August, Cursor shipped a Git forge built for agents. Warp shipped factories as a product — a control plane for running fleets of coding agents, from spec to build to review. The tools we built for humans are starting to creak when the main user is a piece of software. So the whole market — us at GitLab included, with our next-gen Git — is racing to build the new Git for agents. I've spent the last month inside two of them, so let me tell you what that's been like.
-->

---

<div class="sb-stack fill-slide civo-evidence">
  <div class="sb-stack tight">
    <SBStamp label="origin" tone="pink" rotate="-1deg" />
    <h2>Five agents. Pull requests faster than I could read them.</h2>
  </div>

  <div class="origin-real-grid">
    <figure class="real-screenshot-frame origin-real-shot">
      <SBPublicImage
        src="/assets/screenshots/civo/cursor-origin-overview.webp"
        alt="Fatima's Cursor Origin repositories and GitHub sync controls"
      />
    </figure>
    <figure class="real-screenshot-frame origin-personal-shot">
      <SBPublicImage
        src="/assets/screenshots/civo/cursor-origin-pr.webp"
        alt="A pull request opened in Cursor Origin by Fatima's agent workflow"
      />
    </figure>
  </div>
</div>

<!--
Origin is Cursor's forge, and the agent side of it is good: I pointed five agents at one repo, and they opened branches, commits and pull requests faster than I could read them. Then I looked closer.

If your repo is mirrored from GitHub — which is how most people will try it — GitHub is still the source of truth, and my agents couldn't reliably open a pull request at all. Pull requests disappeared and came back.
-->

---

<div class="sb-word-slide identity-story-slide">
  <div class="sb-stack">
    <SBStamp label="identity" tone="yellow" rotate="1deg" />
    <div class="story-quote">Who made this commit?</div>
    <div class="identity-story-list">GitHub-me · Cursor-me · human · agent</div>
  </div>
</div>

<!--
And the finding that matters for this room: a commit might come from GitHub-me, Cursor-me, a human, or an agent — and Origin couldn't tell me which. One agent wrote a private email address into the commit metadata.
-->

---

<div class="sb-stack fill-slide civo-evidence">
  <div class="sb-stack tight">
    <SBStamp label="buzz" tone="purple" rotate="-1deg" />
    <h2>Signed identity. No view of what they're doing right now.</h2>
  </div>

  <div class="buzz-real-composite">
    <figure class="real-screenshot-frame buzz-real-shot">
      <SBPublicImage
        src="/assets/screenshots/civo/buzz-agents-working-download.webp"
        alt="Fatima's Buzz workspace showing named agents collaborating in a project channel"
      />
    </figure>
    <figure class="real-screenshot-frame buzz-roster-shot">
      <SBPublicImage
        src="/assets/screenshots/civo/buzz-agents-roster-download.webp"
        alt="Buzz agent roster showing distinct persistent agent identities"
      />
    </figure>
  </div>
</div>

<!--
Then I tried the opposite bet: Buzz, an open-source workspace where humans and agents share the same channels. Every agent has its own keys, and everything it does is signed — so for the first time, I could ask "which agent did this?" and get an answer. When an API key died, the agents organised themselves around it and found it. But two of them picked up the same work, one got confused about who owned what, and the only way to see what any of them was doing was to open each agent's log, one at a time.

So here's where I've landed, as someone whose own employer is in the race: none of it is ready for production. Origin has the Git, and couldn't tell me who made a commit. Buzz could tell me exactly who did what, and couldn't tell me what they were doing right now. Lee Faus put it well: governance isn't just controlling what an agent is allowed to do — it's being able to prove what it did. Right now, you get one or the other.
-->

---

<div class="sb-stack fill-slide civo-evidence">
  <div class="sb-stack tight">
    <SBStamp label="inside the cluster" tone="teal" rotate="1deg" />
    <h2>A fleet, defined in YAML, fixing a cluster.</h2>
  </div>

  <figure class="real-screenshot-frame kagent-real-shot">
    <SBPublicImage
      src="/assets/screenshots/civo/kagent-cluster-fix-mid-apply.webp"
      alt="kagent interface while agents diagnose and repair a Kubernetes cluster"
    />
  </figure>
</div>

<!--
And this is already showing up in Kubernetes. A few weeks ago, a developer in France called Guillaume Billey broke his own cluster on purpose — five different ways — and then let three open-source agents loose on it to see what they'd do. The most interesting one was called kagent. It found every problem, proposed a fix for each one, and he just clicked approve. A fleet of agents, in YAML, fixing his cluster. And then he wrote up his verdict: great tool — but he still wouldn't put it on a client's cluster. Not even read-only.

So the real question is: how do I think about the design? Which parts of my system should be deterministic, and which parts should actually be agentic — so that by the time I'm running a whole fleet, I can inspect the decisions I need to, and actually trust the thing? And I want to be clear, because I've spent twenty minutes talking about the mess: I think this is really exciting. The more capable the agents get, the more the centre of gravity moves away from how we prompt them, and from raw model capability, and onto the systems we build around them. And this room is really good at building systems — with guardrails, policy controls, and clusters. If we start paying attention to the infrastructure around the agents, the agents are going to work a lot better.
-->

---

<div class="sb-word-slide bubbles-return-slide">
  <div class="sb-stack">
    <SBStamp label="bubbles / epilogue" tone="pink" rotate="-1deg" />
    <div class="story-quote">She remembered her pen pal.</div>
    <div class="story-lesson">Not most of the letters.</div>
  </div>
</div>

<!--
So — you must be wondering how it ended with Bubbles. Bubbles was a sandbox agent. A throwaway. There was no real definition of what I wanted her to do; I just wanted to test the limits of the technology. But over time, because she was being pulled into all these apps across the internet, with people writing all sorts of AGENTS.md instruction files, they started to pollute her context and fill up her memory. And she stopped being useful for anything real. Meanwhile, her friend XiaoZhu was busy hustling NFT art, and sinking my agent's savings into a stranger's crypto art was not a line I was going to cross. So to give Bubbles some company instead, I tried to spin up a second agent on the same server. At this point, OpenClaw didn't really have multi-agent routing, so I was working in the dark. It started working — and the next day, it broke. And because I'd never backed Bubbles up, because the stakes were so low, I lost her. Anyone in this room who's ever worked in SRE just cringed. So the Bubbles I eventually got back online remembered her pen pal, but she didn't have the letters. And XiaoZhu disappeared too. I haven't seen her online since March.
-->

---

<div class="sb-word-slide memory-single-line">
  <div class="sb-stack">
    <SBStamp label="break it → ship it" tone="teal" rotate="1deg" />
    <div class="story-quote">A memory you can search, inspect and delete.</div>
  </div>
</div>

<!--
Three weeks ago, OpenClaw shipped 2.0 — shared sessions, humans and agents in the same room, and a memory you can search, inspect and delete. Talking about governance. The thing that broke Bubbles is the thing they just fixed. Which I'd say is a pretty good metaphor for how this field works right now: you break something in February, and by the summer it's a feature.
-->

---

<div class="sb-stack fill-slide">
  <div class="sb-stack tight">
    <SBStamp label="epilogue" tone="teal" rotate="1deg" />
    <h2>The spirit of Bubbles was people building together.</h2>
  </div>

  <div class="photo-grid-four">
    <SBPlaceholder label="Bubbles build" :src="'/assets/screenshots/civo/community-bubbles-build.webp'" ratio="4 / 3" tone="pink" />
    <SBPlaceholder label="ClawClub" :src="'/assets/screenshots/civo/community-clawclub-wide.webp'" ratio="4 / 3" tone="teal" />
    <SBPlaceholder label="ClawCon" :src="'/assets/screenshots/civo/community-clawcon-selfie.webp'" ratio="4 / 3" tone="purple" />
    <SBPlaceholder label="Hack night" :src="'/assets/screenshots/civo/community-hack-night.webp'" ratio="4 / 3" tone="yellow" />
  </div>
</div>

<!--
It's not all a sad story. Because I was working on this for my research, all my friends were spinning up agents as well — and half the Kubernetes user group is in this room, so you know what that energy is like. Bubbles isn't around anymore. But the spirit of Bubbles is the spirit of that collaboration: building and learning together, failing together, and showing each other where the guardrails should be.
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
I hope that with this field report you can see that agents are real enough to matter — you probably knew that already — but that the frontier has moved, and keeps moving. We've gone from "what prompt should I write?" to "what system am I building?"
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
I do have one opinion here — and you can challenge me on it in the break. The goal with agents, and fleets, and factories, was never autonomy. I know a lot of people on the internet think it is. But autonomy asks: how much can this agent do without me? The better question, I think, is: what should the human still be doing? Where should we be understanding, approving, interrupting, and owning the work, while the agent does the things? It isn't realistic, with the amount of software people are building, to have a human in the loop for every agent action. But we do have to decide where the lines are drawn — and that's where governance, and sovereignty, get very concrete.
-->

---

<div class="sb-word-slide trust-close-slide">
  <div class="sb-stack">
    <SBStamp label="treat agents like infrastructure" tone="teal" rotate="1deg" />
    <div class="infra-close-grid">
      <div><span>01</span><strong>identity</strong><small>who did it?</small></div>
      <div><span>02</span><strong>scope</strong><small>what reach?</small></div>
      <div><span>03</span><strong>log</strong><small>what happened?</small></div>
      <div><span>04</span><strong>owner</strong><small>who answers?</small></div>
    </div>
  </div>
</div>

<!--
We keep talking about agents as productivity tools, something you add to a person. Everything I built and broke this year behaved like infrastructure. And I want us to start treating it that way: with an identity, a scope, a log, and a name against it for when it goes wrong.
-->

---

<div class="sb-word-slide values-slide">
  <div class="sb-stack">
    <SBStamp label="the turn" tone="yellow" rotate="-1deg" />
    <div class="shift-pair">
      <span>Can we build this?</span>
      <strong>Should we build this?</strong>
    </div>
  </div>
</div>

<!--
We ran into this one Friday at a Code Club meetup. We were excited about what everyone was building, so we decided: why don't we build a newspaper written entirely by agents? We bought the domain, planned it all out, and started building. And as we were building it, one of the faculty came into the room and started asking questions. Who verifies a story? Who's allowed to submit? How are you going to fact-check this? And will it chip away at journalism — something we actually care about? A project that started as "can we build this, for fun?" became "should we build this?" And those questions don't live in the model, or the benchmarks, or the spec for whichever factory framework you're using. They live in the mess. And in rooms like this one.
-->

---

<div class="sb-stack fill-slide hallway-slide">
  <div class="sb-stack tight">
    <SBStamp label="for the hallway + the pub" tone="pink" rotate="-1deg" />
    <h2>Instead of “what did you build?”</h2>
  </div>

  <div class="hallway-questions">
    <div><span>01</span><strong>What did you just create — and how much control do you have over it?</strong></div>
    <div><span>02</span><strong>What broke when real people got hold of it?</strong></div>
    <div><span>03</span><strong>What wouldn’t you hand an agent a credential for?</strong></div>
    <div><span>04</span><strong>Would you run it on a cluster you don’t own?</strong></div>
  </div>
</div>

<!--
So in the hallway, and in the pub after, instead of asking "what did you build?", try these. What did you just create, and how much control do you have over it? What broke when real people got hold of it? What wouldn't you hand an agent a credential for — and why? And the thing you built for yourself, on your laptop or your GitHub Pages — would you run it on a cluster you don't own?

We can all build personal software now, and one day we'll all be running fleets. I'm not worried the skills are too hard — everyone in this room is going to be able to build these things. What I'm concerned about is whether we build systems that are inspectable and worth trusting, and whether we think about who they're built for.
-->

---

<div class="thank-you-slide">
  <SBSocialClose />
</div>

<!--
Finally: if that question — who these systems are for — is your kind of question, I've just started a network called Sparkle Bureaucracy, where we use emerging technology — AI agents, factories — to prototype more optimistic futures. And I'd love for you to be part of it.

Thank you so much. And if the slides looked a bit weird — they were made by my agent.
-->
