# Squeeze experiment

Baseline: tag `v-full` on `main`. Return there if this branch degrades behaviour.

## The split

Compressibility and necessity run opposite to each other. A rule compresses well
when the model already knows it and would act on it anyway — but then the rule
was nearly free to delete. A rule resists compression when the model's trained
default pulls the other way, and those are the rules doing the work.

| Class | Meaning | Treatment |
| --- | --- | --- |
| **Default conflict** | The model's habit pulls the other way | Do not squeeze |
| **Salience gap** | The model can, it just does not think to | A short cue is enough |
| **Capability gap** | The model does not know how | Keep the demonstration |

## Repair rule

If a squeezed item degrades in practice, the split was wrong for that item.
Promote it one step toward Capability gap — a cue becomes a specification, a
specification becomes a demonstration — rather than reverting the whole branch.

## Squeezed (salience gap)

- `Before you act outside the task` — permission list collapsed to one sentence
- `When you touch the user's files or state` — two paragraphs merged
- `When you leave work behind` — dropped the generic maintainability enumeration
- `Match the rigour to the consequences` — high-stakes categories collapsed
- `Design the representation` — trimmed the enumerations of forms
- The long-or-multi-step-context paragraph

## Deliberately left alone (default conflict)

These fight what models do by default. They stay specified.

- "Report the result and its meaning, not a timeline of what you did" + the omit list
- "When your text ends, your turn ends" and never describing progress as continuing
- "A check on something that would look identical if the claim were false is not a check"
- "A failed attempt must change the diagnosis before anything else changes"
- "Never mix the options into a sentence or a solid text block"
- "Structure comes first ... do not imitate brevity with fragments"
- "Change only what the result requires" (scope creep)

## Left alone (capability gap)

- The Language Example. Demonstration is the mechanism; a cue cannot replace it.
