# Chapter 8: Is It Done Yet?

No.

Software is never done. Not really. This is the fundamental frustration and the fundamental truth of software development. You can ship it, release it, deploy it to production, mark the ticket as closed, and move on to the next project. But the software itself is never truly finished.

There's always one more bug. One more feature. One more optimization. One more edge case. One more user requesting one more thing.

The question isn't "Is it done?" The question is "Is it good enough to ship?"

## The Myth of Completion

In traditional manufacturing, products have a finished state. You build a chair. When the chair is complete, you're done. It might need maintenance or repairs later, but the act of creation is complete. The chair is finished.

Software doesn't work this way.

You build version 1.0 of your application. It works. You ship it. Users start using it. Then:

- They find bugs you didn't anticipate
- They request features you didn't think of
- The technology stack gets updates that break compatibility
- Security vulnerabilities are discovered
- Competitors launch features you need to match
- The business changes and requires new functionality
- The platform (web browser, OS, mobile device) evolves
- User expectations rise as they experience other software

Your "finished" product is already becoming obsolete. To keep it viable, you need to maintain it, update it, improve it. Forever.

This is why software companies have recurring revenue models. Software-as-a-Service isn't just a business model; it's an acknowledgment of reality. Software is never a product; it's a service that happens to involve code.

## The Art of Shipping

Given that software is never truly done, how do you decide when to ship?

**The Minimum Viable Product** philosophy says: ship the smallest thing that provides value, then iterate based on feedback. Don't build features nobody wants. Don't polish things that don't matter. Ship early, learn fast.

This works well for startups. It fails catastrophically for medical devices, aviation software, or financial systems where "iterate based on feedback" might mean "people died, let's fix that in the next release."

**The Feature Complete** approach says: define what "done" means upfront, build all those features, then ship. This provides clarity and ensures you're delivering what was promised. But it's slow, and by the time you ship, requirements might have changed.

**The Time-Boxed Release** approach says: we'll ship whatever's ready in 6 weeks (or 3 months, or whatever). Some features will make it, some won't. This creates predictable cadence and forces prioritization. But it might mean shipping incomplete features or delaying important ones.

**The "When It's Ready"** approach says: we'll ship when it meets our quality standards, however long that takes. This is how Blizzard used to work, and how some open source projects work. It produces polished products but can lead to massive delays and scope creep.

None of these is objectively correct. The right approach depends on what you're building and who you're building it for.

But in every case, "done" is a decision, not a state. Someone decides that the software is good enough to ship, knowing that it's not perfect, and that work will continue after release.

## The Technical Debt Tax

Every shortcut you take while building software creates technical debt—work you'll need to do later to fix the shortcut.

**Quick and dirty now** means **slow and painful later.**

Examples:

- You hardcode a value instead of making it configurable. Later, when requirements change, you need to refactor.
- You skip writing tests because you're in a hurry. Later, when you need to change the code, you're afraid of breaking things.
- You copy-paste code instead of creating a reusable function. Later, when you find a bug, you need to fix it in five places.
- You choose a technology because it's trendy, not because it's appropriate. Later, you're maintaining a complex system you don't understand.
- You ignore performance because it's "good enough." Later, when you have more users, everything is slow and you need to rewrite.

Some technical debt is worth it. If you're validating a business idea, quick-and-dirty is fine. If the project might be cancelled next month, don't over-engineer it.

But debt accumulates. Interest compounds. Eventually, the codebase becomes so encrusted with shortcuts, workarounds, and patches that making any change is risky. This is how you get legacy systems that nobody dares to touch.

The "done" that lets you ship faster now creates the "undone" that slows you down later. Balancing these is the art of software development.

## The Bug Queue Is Infinite

Here's a depressing realization: you will never fix all the bugs.

Every software project above trivial size has a bug queue. Users report issues. QA finds problems. Developers notice edge cases. The queue grows.

Some bugs get fixed immediately—crashes, data loss, security vulnerabilities. These are critical.

Some bugs are annoying but not critical. They get prioritized based on how many users they affect, how often they occur, and how hard they are to fix.

Some bugs are so minor that they'll never be fixed. "The text on this button is slightly misaligned on this one specific browser in dark mode when you have accessibility settings enabled." Sure, it's a bug. No, we're not fixing it. We have ten thousand more important things to do.

And some "bugs" are actually feature requests in disguise. "The app doesn't do X" might be reported as a bug, but it's really a request for new functionality that was never planned.

The bug queue is triage. Constant triage. You're always deciding what's important enough to fix and what you'll live with. This is emotionally difficult for developers who want things to be correct. But it's necessary.

Perfectionism is the enemy of shipping. You can have perfect software or shipped software, but rarely both.

## The Maintenance Phase That Never Ends

In traditional project management, there's a "maintenance phase" that comes after development. You build the software, ship it, and then switch to maintenance mode—just fixing bugs and keeping it running.

In reality, most software is always in maintenance mode. You're always fixing bugs from previous releases while adding features for the next release. Development and maintenance happen simultaneously.

And maintenance is harder than development in many ways:

**You're working with existing code,** possibly written by someone else, possibly years ago. Understanding what it does and why is difficult.

**You can't break things.** In new development, if something doesn't work, you fix it. In maintenance, if you break something that was working, users complain. Your changes need to be surgical—fix the problem without disturbing anything else.

**You're dealing with real users and real data.** In development, you work with test data. In maintenance, you're working with production systems that people depend on. The stakes are higher.

**You inherit all the technical debt.** Every shortcut, every hack, every "we'll fix this later"—you're the one who has to live with it now.

Some developers love maintenance—it's detective work, puzzle-solving, and optimization. Others hate it—they want to build new things, not fix old ones.

But someone has to do it, because software is never done, which means it always needs maintaining.

## The Scope Creep Monster

You define what you're building. You estimate how long it will take. You start building.

Then someone says, "While you're at it, could you also...?"

Scope creep is the gradual expansion of a project beyond its original goals. It's the reason projects run late and budgets explode. It's also nearly inevitable, because requirements are discovered, not known upfront.

The conversation goes like this:

**Developer:** "The feature is almost done. Should be finished by Friday."

**Stakeholder:** "Great! Oh, one thing—can it also handle edge case X?"

**Developer:** "That's... a different feature, actually. That would require—"

**Stakeholder:** "But it's related! Users will expect it to work that way."

**Developer:** "Right, but that wasn't in the original requirements..."

**Stakeholder:** "Well, now that we're thinking about it, it seems obvious. How long would it take?"

**Developer:** *internally screaming* "Maybe another week?"

**Stakeholder:** "Let's just add it. We're so close anyway."

Multiply this conversation by a dozen features and you see how a two-month project becomes a six-month project.

The solution is supposed to be clear requirements, change management processes, and the discipline to say "no, that's out of scope." In practice, requirements are always incomplete, processes get circumvented, and "no" is politically difficult.

So we do our best to manage scope creep, knowing that we'll never eliminate it entirely. The question "Is it done?" gets answered with "Define 'it.'"

## The Release Anxiety

Shipping software is stressful. No matter how much you've tested, something might go wrong. Deployments are acts of faith.

**The pre-release checklist:**
- Did we test all the features?
- Did we test on all the platforms?
- Did we check for security vulnerabilities?
- Did we review the code?
- Did we update the documentation?
- Did we communicate with users about the changes?
- Did we have a rollback plan?
- Did we sacrifice to the appropriate deities?

You go through the checklist. Everything looks good. You deploy.

Then you watch. Monitoring dashboards. Error logs. User feedback. Waiting for something to break.

Usually, everything is fine. Sometimes, something breaks—a bug you didn't catch, an edge case you didn't think of, an interaction between systems you didn't anticipate.

This is why experienced developers never deploy on Friday. If something breaks, you want time to fix it before the weekend. You definitely don't want to be debugging production at midnight on Saturday.

The anxiety lessens with experience, but it never entirely goes away. Every release is a little bit scary, because once it's in production, it's real. People are using it. If it's broken, you need to fix it now, not next sprint.

## The Paradox of "Finished" Features

Here's a strange truth: finishing a feature often reveals more work.

You build the feature. It works. You ship it. Users start using it. Then they discover:

- It doesn't quite work the way they expected
- It's missing functionality they assumed would be there
- It interacts badly with another feature
- It's slower than they need
- It works on desktop but not mobile
- The UI is confusing
- It needs better error messages
- It needs configuration options
- It needs documentation
- It needs tutorials

The feature is "done" in the sense that the code is written and it works as designed. But it's not done in the sense of meeting user needs completely.

This is where the iterative approach helps. Version 1 is done, but version 2 will be better. Version 3 even better. Each iteration gets closer to what users actually need, which is often different from what they initially said they wanted.

Software is never finished; it's only released.

## The Sunset

Eventually, some software does reach an end state: abandonment.

**The project is cancelled.** The business pivots, funding runs out, or someone realizes the idea wasn't viable. The code goes into a repository somewhere and is never touched again.

**The software is deprecated.** A newer, better solution exists. Users are migrated to the replacement. The old software is shut down. This is a good ending—the software fulfilled its purpose and was succeeded by something better.

**The software dies from neglect.** Nobody maintains it. Dependencies break. It no longer runs on modern systems. Eventually, it stops working entirely and nobody bothers to fix it.

**The software becomes legacy.** It still runs, but nobody wants to touch it. It works just well enough that replacing it isn't worth the cost. It enters a zombie state—neither alive nor fully dead.

This is the only real "done" for software: when it stops being used, stops being maintained, and fades into digital archaeology.

But until that happens, the software is a living thing, constantly evolving, never quite finished.

## Making Peace With Incompletion

The hardest thing for new developers to accept is that their work will never be perfect. There will always be bugs you didn't fix, features you didn't implement, code that could be cleaner, designs that could be better.

You have to make peace with this. You have to accept "good enough" even though you can see all the ways it's not good enough.

This isn't settling for mediocrity. It's recognizing that done is better than perfect, that shipped software creates value while perfect software sitting on your laptop creates none.

It's understanding that software development is a series of trade-offs: speed vs. quality, features vs. simplicity, flexibility vs. performance. Every decision is a compromise.

It's acknowledging that you're building for humans, who are messy and contradictory and will use your software in ways you never imagined. You can't anticipate everything. You can only do your best and iterate.

**The Zen of Shipping:**

- Ship when it's good enough, not when it's perfect
- Fix the critical bugs; live with the minor ones
- Prioritize ruthlessly; you can't build everything
- Accept that you'll need to maintain it forever
- Plan for the next version instead of trying to make this version complete
- Measure success by value delivered, not features built
- Remember that real users with real problems is better than imaginary users with imaginary perfection

Software is never done. That's not a failure; it's the nature of the medium.

The question isn't "Is it done yet?"

The question is "Have we delivered enough value that we can call this a success?"

And when the answer is yes, you ship it. Knowing full well that tomorrow, you'll be working on the next version.

Because it's never done.

And that's okay.

But what about the software that was "done" years ago, written by people who've moved on, and is now your problem to maintain? That's a special kind of challenge, and it's where most developers spend most of their time.

---

*Next: Chapter 9 - [Legacy Code and Digital Archaeology](chapter-09-legacy-code.md)*
