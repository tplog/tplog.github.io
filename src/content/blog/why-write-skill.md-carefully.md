# Why Skill Directory Structure Matters

**Writing Skills for AI agents is essentially memory management.** The context window is your limited resource. Use it poorly and the model slows down, misses key points, or forgets instructions. Structure your Skill well and the model stays focused and efficient.

---

## The problem: context is expensive

LLM attention cost grows quadratically with context length. 2,000 tokens does not cost 2x the compute of 1,000 tokens—it can cost 4x.

Some developers dump everything into one giant `skill.md` file. The model "works," but it carries that entire weight on every single call. It is like forcing every program instruction through L1 cache alongside the data. Waste.

## The solution: structured Skills as multi-level cache

Treat your Skill directory like a computer memory hierarchy:

| Level | File | Purpose |
|-------|------|---------|
| L1 | `skill.md` | Core workflow, principles, pointers—always loaded |
| L2/L3 | Subdocs, templates | Details loaded on demand |
| Disk | External knowledge | Retrieved via RAG only when needed |

The main `skill.md` should act as a **router**: "If X happens, read file Y. If Z happens, use tool W."

Keep the L1 cache small. Move detailed specs, templates, and edge cases to separate files. The model fetches them only when relevant, preserving precious context space for actual problem-solving.

---

## Bottom line

Engineers used to count bytes in memory. Today we count tokens in context windows. Different constraints, same discipline: **put critical information where it belongs and keep the hot path clean.**

Until AI context becomes truly unlimited, thoughtful Skill structure remains essential for anyone building serious agent workflows.
