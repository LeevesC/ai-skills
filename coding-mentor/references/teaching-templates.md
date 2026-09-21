# Teaching templates

Pick one based on which kind of concept it is (see SKILL.md for how to tell). These are shapes to adapt, not fill-in-the-blank forms — skip a section if it's genuinely not useful for a given concept, but don't skip the "why" section, since that's the whole point of this skill.

## Spec Template — Language/runtime mechanism

Use for: things baked into a language or runtime (Promises, closures, garbage collection, generators, SQL window functions, hoisting, virtual DOM diffing, etc.)

1. **The problem, before this existed.** What did developers have to do before this mechanism existed, and what was painful/error-prone/verbose about it? Be concrete — a tiny "here's what this used to look like" beats an abstract description.
2. **What it was built to fix.** Name the specific pain point(s) from step 1 that this mechanism directly targets.
3. **How it works.** Now the mechanics — walk through it step by step, checking in as you go (see SKILL.md's "how to teach" section). This is where a diagram or before/after snippet pays off most.
4. **Where it shows up in practice.** A short example grounded in the user's actual stack (check `tech_skill.md`), not a generic textbook example.
5. **Common trip-ups.** One or two things people new to this get wrong, briefly.

## Practice Template — Engineering/real-world concept

Use for: things that solve a problem regardless of language (lazy loading, payload tamper-proofing, idempotency, caching invalidation, rate limiting, eventual consistency, feature flags, etc.)

1. **The real-world problem.** Describe a concrete scenario — ideally one plausible in the user's own context — where this problem shows up. Make it specific enough to picture, not a one-line abstract definition.
2. **What goes wrong without it.** Walk through what actually happens/breaks/gets messy if you don't apply the concept. This is the part generic explanations skip, and it's the part that makes the concept stick — show the mess, don't just assert it exists.
3. **How the concept fixes it.** Introduce the concept now that the pain is established, and connect each part of the fix back to a specific piece of the mess from step 2.
4. **What it looks like in code/practice.** A grounded example in the user's stack where relevant, or a description of what implementing it would involve if it's more architectural than a single snippet.
5. **Trade-offs.** Most engineering concepts aren't free — briefly note what you give up or add in complexity by using it.

## Concepts with both flavors

Some concepts (async/await, memoization, ORMs) have a language-mechanism side and a real-world-problem side. Lead with whichever makes the motivation click faster for the specific concept, and fold in a shorter pass of the other template rather than running both in full.
