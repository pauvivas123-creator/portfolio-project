Post 1
Linkedin
4 hours.

Anthropic shipped Claude Managed Agents last week and most people missed what actually changed.


So here's a simple way to think about it.

Every workflow your team runs falls into one of two buckets: 

tasks that require a human to initiate them every time, and tasks that just need to happen.

Most teams have the second bucket full of things still sitting in the first one.

That's the gap agents close.

Here's how we're applying this at Understory:

Outbound: Lists get pulled, enriched, sequenced, and pushed into HubSpot automatically. Someone still sets the strategy. Nobody has to fire the gun every morning.

Client onboarding: There are 15 steps between a signed contract and a live campaign. Most of them are execution. An agent with persistent memory runs those steps overnight. A human manages the relationship.

CRM hygiene: Nobody cleans data because nobody has time to clean data. An agent does it every week, logs every change, flags what needs a human eye. It just runs.

Content research: The agent monitors client industries, finds angles, drafts in their voice, and queues posts for review. The team edits. Nobody starts from a blank page.

Campaign reporting: Daily performance summaries, CPL alerts, client-ready reports delivered before anyone asks. The work happens whether or not someone remembers to pull it.

The pattern across all five: the agent owns the execution loop, the human owns the judgment.

That's where the real leverage is. Not in replacing your team - in clearing the work off their plate that was never a good use of their time to begin with.

Post 2:
linkedin
6 days.

You are probably spending 5x more on AI than you need to.


Not because the models are expensive (even though they are). Because you're running the wrong model on the wrong tasks.

Extremely timely news after my last post about Opus getting a math problem wrong, Anthropic just shipped something called the Advisor Tool.

Here's the architecture in plain English:

You run Haiku on everything. When it hits a hard decision, it calls Opus for help.

Opus answers. Haiku keeps going. One API flag. No extra infrastructure. No code overhaul.

These are the results on BrowseComp, which is Anthropic's benchmark for complex multi-step research tasks, the kind that require 10+ searches to find a hard answer:

Haiku alone: 19.7% of questions answered correctly.
Haiku + Opus Advisor: 41.2% of questions answered correctly.

More than double the accuracy. At 85% lower cost than running Sonnet on the same tasks.

Then when it comes to coding, Haiku 4.5 measures at 73.3% vs Sonnet 4.6 at 79.6% and Opus 4.6 at 80.8%.

Why does this matter for GTM teams specifically?

Your outbound agents, lead enrichment flows, and HubSpot automations are doing research constantly. Finding the right contact. Pulling the right signal. Deciding whether to engage.

That is exactly what BrowseComp measures.

And right now, most teams are running Sonnet or Opus on 100% of those decisions.

Here is what the model tier actually looks like today:

Haiku 4.5: $1 input / $5 output per million tokens
Sonnet 4.6: $3 input / $15 output per million tokens
Opus 4.6: $5 input / $25 output per million tokens

Haiku is 5x cheaper than Opus on input. 5x cheaper on output.

With the Advisor Tool, you get near-Opus accuracy on the decisions that matter. Haiku pricing on everything else.

Most GTM teams obsess over prompt engineering.

Almost nobody is looking at model selection.

The teams that figure out which five workflows should just happen automatically, and actually build that, will be running circles around everyone still doing it manually by the end of the year.
