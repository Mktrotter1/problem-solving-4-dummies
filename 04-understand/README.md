# Step 4: Understand

> *Why is it happening?*

You know what the problem is. Now figure out *why* it exists. This is the difference between treating symptoms and curing disease.

## What This Step Is

Understanding means finding the root cause — the thing that, if you changed it, would make the problem go away. Not the thing that's most visible. Not the thing that's most annoying. The thing that's actually *causing* the situation.

## How to Do It

**Ask "why?" until you hit bedrock.** The surface answer is almost never the real answer. Keep digging.

**Check your assumptions.** List every assumption you're making. Then question each one. "Is this actually true, or have I just been assuming it?" Many problems exist because of an assumption nobody ever verified.

**Map the relationships.** How do the parts of this problem connect? What depends on what? What triggers what? Draw it if you have to — visual maps externalize complexity that your brain can't hold.

**Look for the system, not just the event.** A single failure is an event. But events happen inside systems. What about the system allowed or caused this event? That's where the leverage is.

## Techniques That Help Here

### The 5 Whys
Ask "Why?" iteratively, typically five times, to drill from symptom to root cause.

> "The server went down." Why?
> "It ran out of memory." Why?
> "The cache grew without limit." Why?
> "There's no eviction policy." Why?
> "Nobody defined one when the cache was added." **Root cause.**

Rules: follow one causal chain at a time. If you branch, pick the most likely path and trace it fully before trying others. Stop when "why?" no longer produces a meaningful, actionable answer.

### First Principles Thinking
Strip away everything you've been told about the problem and ask: what do I know to be *fundamentally true*? Build your understanding up from only those truths.

This is especially powerful when everyone "knows" why something is the way it is, but nobody has actually verified it. Convention and root cause are not the same thing.

### Fishbone Diagram (Ishikawa)
For complex problems with multiple possible causes, map them by category:

```
People ──────┐
Process ─────┤
Equipment ───┼──▶ [THE PROBLEM]
Materials ───┤
Environment ─┤
Management ──┘
```

Useful when the cause isn't obvious and you need to systematically survey the landscape.

### Cynefin Framework (Problem Classification)
Before going deep on root cause analysis, check what *kind* of problem you're dealing with:

- **Clear:** Cause is obvious. Just follow best practice.
- **Complicated:** Cause exists but requires expertise to find. Analyze, then respond.
- **Complex:** Cause-and-effect can only be seen in hindsight. You have to probe (experiment) to understand.
- **Chaotic:** No cause-and-effect relationship is perceivable. Stabilize first, understand later.

This matters because using "complicated" tools (deep analysis) on a "complex" problem (emergent behavior) is a common and expensive mistake. If analysis isn't converging on an answer, you might need experiments instead.

## Common Mistakes

- **Stopping at the first "why."** The first answer is almost always a symptom, not a cause.
- **Confusing correlation with causation.** "It started failing after the deploy" doesn't mean the deploy caused it. It might. Verify.
- **Anchoring on a pet theory.** If you're attached to an explanation, you'll unconsciously filter evidence to support it. Actively look for evidence that *disproves* your theory.
- **Ignoring the human/system layer.** Technical problems often have organizational root causes. "Why was there no eviction policy?" might lead to "because there's no review process for caching changes."

## The Key Question

**"If I changed [this cause], would the problem go away?"**

If you can answer that with confidence, move to [Step 5: Define Done](../05-define-done/).
If not, keep digging — or consider that you're dealing with a complex/chaotic problem that needs experimentation, not analysis.
