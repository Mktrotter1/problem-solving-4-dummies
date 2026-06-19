# Step 5: Define Done

> *What does solved look like?*

You know what's wrong and why. Before you generate solutions, define the target. If you don't know where you're going, you'll either wander forever or declare victory too early.

## What This Step Is

Defining done means creating a clear, testable description of the world after the problem is solved. Not vague aspirations — concrete conditions you can check.

This step gets skipped more than any other. And when it's skipped, you get scope creep, endless tinkering, "good enough" compromises, and solutions that technically work but don't actually solve the problem.

## How to Do It

**Describe the end state, not the method.** "Customers can complete checkout in under 60 seconds" — not "rewrite the checkout page." The end state is fixed; the method is flexible.

**Make it testable.** If you can't verify whether you've achieved it, it's not defined well enough. "Better performance" isn't testable. "Page loads in under 2 seconds on 3G" is.

**Define the boundary.** What's in scope? What's out? "Solved" doesn't mean "perfect." It means "good enough that this specific problem no longer exists."

**Identify constraints.** What are you not willing to sacrifice? Time, money, quality, safety, simplicity? Name them now, before solutions start competing for your attention.

**Write acceptance criteria** — the concrete, checkable conditions that together make up your definition of done. Literally write: "I will consider this solved when ___." Fill in the blank with observable, measurable conditions.

**If you're running an experiment** — a complex problem with no clear root cause (see [Step 4](../04-understand/)) — define done as what you expect to *learn*, not what you expect to fix. "We'll know whether the cache is the bottleneck" is a valid done for a probe.

## Techniques That Help Here

### Inversion (Defining the Anti-Goal)

Instead of (or in addition to) defining success, define failure. "What would definitely mean this is NOT solved?" This creates a floor — a minimum bar that any solution must clear.

Charlie Munger: *"Tell me where I'm going to die, and I'll never go there."*

### Working Backward

Start from the solved state and trace backward. "If the problem were solved, what would be true? And for that to be true, what else would need to be true?" This reveals hidden requirements and dependencies.

## Common Mistakes

- **Skipping this step.** The most common mistake. You *feel* like you know what done looks like, so you don't write it down. Then three hours later you realize you and everyone else had different pictures of "done."
- **Setting the bar too high.** "Done" is not "perfect." It's "the problem is no longer a problem." Perfection is the enemy of solved.
- **Setting the bar too low.** "Done" is not "I did something." The problem must actually stop being a problem.
- **Conflating the solution with the goal.** "Deploy the new service" is a task, not a definition of done. "API response times are under 200ms at p99" is a definition of done.

## The Key Question

**"How will I know — concretely, testably — that this problem is solved?"**

Write it down. Then move to [Step 6: Generate Options](../06-generate-options/).
