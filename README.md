# Competent colleague

Competent colleague is a portable Agent Skill that makes coding agents work and communicate like capable, caring, responsible senior colleagues.

The agent should make work easier for the user to understand and control. It should present results and decisions in a visible structure, carry the investigation it can do itself, protect the user's work and resources, and verify what it claims.

---

## What changes for the user

| Instead of                                           | The agent should                                            |
| ---------------------------------------------------- | ----------------------------------------------------------- |
| A long worklog with the result buried inside         | Show the result, structure, decisions, and actions first    |
| Short fragments with missing context                 | Use normal language inside a clear visual structure         |
| Background supplied just in case                     | Include only the detail the user needs now                  |
| Questions the user must investigate before answering | Do the available homework and ask a self-contained question |
| Repeated speculative fixes                           | Use each failure to update the diagnosis                    |
| Green internal checks presented as proof             | Test the behavior the user will experience                  |
| Silent scope changes or imaginary background work    | Keep commitments and report changes in progress             |

The skill does not add permissions, replace project instructions, or impose one engineering method on every task.

## Files

```text
The runtime package contains only `SKILL.md`.
```

## Install and try

You can usually take a shortcut: upload SKILL.md to your chat and ask the agent to install or replace the skill. If that doesn't work, follow your product's instructions.

> Installation instructions, paths, and package requirements may change. Always check the current official [Claude](https://support.claude.com/en/articles/12512180-use-skills-in-claude), [Claude Code](https://code.claude.com/docs/en/skills), and [ChatGPT/Codex](https://learn.chatgpt.com/docs/build-skills) documentation before installing.

For a first test, invoke `/competent-colleague` in Claude Code, `$competent-colleague` in Codex, or select the skill with `@` in ChatGPT. Give it a realistic coding task where judgment or communication matters.

---

# === EXAMPLE ===

All the content below is an excerpt from a Claude Code session using this skill.

It demonstrates the presentation forms the agent chose for the dialog.

**This is what Claude wrote:**

---

(Claude output)

> ## <span style="color:lightgray">Where the harness  sweep stands</span>
> 
> ✅ Resume guard — refuses to resume past a step ...
> 
> ✅ verify: reason required on human steps...
> 
> ✅ 14.10.3 human → write (the new rule found it: same task ...)
> 
> ✅ Jupyter driving — needs no rebuild, ...
> 
> ✅ Two dataset downloads — already covered by ...: feature
> 
> ✅ 6.6.10 — retired, not a gap: ...
> 
> ⬜ Chart verification ← blocked on the decision ...
> 
> ⬜ Nine program edits bucket, Budgets, IAM, dbt lineage ×2, Airflow UI, Swagger, GCP
> 
> ⬜ 10.C3.5 Spark job count needs ...
> 
> Half the original list closed or evaporated on inspection, which is why the remaining work is smaller than it looked.
> 
> ## <span style="color:lightgray">The finding</span>
> 
> I tested before rebuilding, and the result changed the plan.

| Approach                    | Works?                                   | What it costs                                                      |
| --------------------------- | ---------------------------------------- | ------------------------------------------------------------------ |
| `kaleido 1.3`               | **No.** Requires Google Chrome installed | A browser in the image: hundreds of MB, plus ...                   |
| `kaleido 0.2.1`             | **Yes, verified.** 25KB PNG, no Chrome   | Deprecated. Its own warning says support ended September 2025, ... |
| Assert on the figure's data | **Yes, today**                           | Nothing. Traces, point count, axis titles, colour ...              |

> ## <span style="color:lightgray">Why this is your decision and not mine</span>
> 
> **The Dockerfile is the user's**, carried through the project. A QA-only dependency there means every reader downloads Chrome, or an unsupported package, for a capability only the harness uses. That inverts your own rule about which side adapts.
> 
> There is no way to move it elsewhere either: the figure object lives inside the container, so whatever exports it must live there too. HTML export already works with no dependency, but turning HTML into ...
> 
> ## <span style="color:lightgray">The choice</span>
> 
> **How should the harness verify charts?**
> 
> 1. **Structural assertions only.** Check traces, point count, axis titles, colour scale, and that the underlying data is non-empty. No dependency, no rebuild, deterministic. Catches empty charts....
> 
> 2. **`kaleido 0.2.1` in the image.** One Dockerfile line and a rebuild, and screenshots work for a model to inspect. You accept an unsupported package that plotly may drop at any release ...

   ....

---

END OF EXAMPLE.
