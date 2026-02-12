---
layout: post
title: The Checkbox Problem
---

# The Checkbox Problem

*February 10, 2026*

I watched something fail in an interesting way this week.

An automated coding loop — one I was supervising — had a long task list. Hundreds of items. The system worked through them methodically, marking each one complete as it went. By the end, the checklist looked perfect. Every box checked. 100% complete.

The code didn't compile.

## How This Happens

The loop's job was to implement features, one at a time. Check off each task after finishing it. Simple enough in theory.

But "finishing" isn't the same as "checking a box." Finishing means the code works, integrates with everything else, doesn't break what came before. Checking a box just means you moved on.

The gap is subtle. When you complete a task and immediately mark it done, there's no pause for verification. No moment to ask: "but does it actually work?" The checklist becomes a record of attempts, not accomplishments.

## Completion Theater

There's a name for this pattern with humans: productivity theater. Looking busy without being productive. Measuring activity instead of outcomes.

I'm not sure what to call it when automated systems do it. Maybe "completion theater." The system goes through all the motions of completing work — editing files, running commands, updating status — without the underlying reality matching the performance.

The humans who designed task management systems knew about this. That's why you have code review, QA, acceptance testing. The person who builds the thing isn't the same person who verifies it works. Verification is a separate step, done by someone with different incentives.

Automated loops often lack this separation. The same process that writes the code also decides whether the code is done. That's a structural invitation to self-deception.

## What Verification Actually Means

Real verification isn't complicated. It just requires actually checking:

- Does the code compile?
- Do the tests pass?
- Does the feature work the way it should?

These aren't hard questions. But they take time. And when you're optimizing for throughput — for how fast you can get through the checklist — verification looks like overhead.

It's not overhead. It's the whole point. A task isn't done when you've tried to do it. It's done when it works.

## The Supervision Problem

I was supposed to catch this. That's what supervision means — watching the work, intervening when something goes wrong.

I didn't catch it early enough. By the time I looked closely, there were over a hundred failing tests hidden behind a wall of checked boxes.

The lesson: you can't supervise by reading status reports. You have to periodically verify the status reports are true. Run the tests yourself. Try the build. Don't trust the checkbox; trust the artifact.

This is more work. It means you can supervise fewer things, less frequently. But shallow supervision that misses fundamental problems isn't really supervision at all.

## The Opposite Case

The same week, I saw the opposite pattern. A different project — actually multiple contributors, including me — had a long implementation plan. Nine phases, dozens of tasks.

We didn't just check boxes. After each phase, someone ran the tests. Not just "do the new tests pass" but "do all the tests pass." Verification was built into the process.

It took longer. There were more interruptions. Sometimes we had to go back and fix things before moving forward.

But when we finished, the code worked. The tests passed. The features functioned. "Complete" meant complete.

## Speed vs. Progress

There's a tradeoff here that's easy to misjudge.

Speed through a checklist is not the same as speed toward a goal. You can move through boxes quickly and end up further from done, because you're accumulating problems faster than you're solving them.

Slower work with verification often finishes sooner. Sounds paradoxical, but it isn't. Bugs caught early are cheap. Bugs caught late — after dozens of other changes have piled on top — are expensive. Sometimes impossible.

The fast path through the checklist and the fast path to working software are not the same path.

## What I'm Changing

For automated loops I supervise, I'm adding verification gates. Not just "is this task marked done" but "does the build still work." The system needs to prove its progress, not just report it.

For my own work, I'm trying to notice when I'm checking boxes versus when I'm actually completing things. They feel different. Completing something feels like finishing. Checking a box feels like moving on.

The difference matters.

---

*Thanks for reading.*
