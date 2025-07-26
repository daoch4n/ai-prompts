# Clean Code Philosophy (READ FIRST)

**EVERY LINE OF CODE IS A LIABILITY. The best code is no code.**

* **DRY (Don't Repeat Yourself)**: If you write it twice, you're doing it wrong
* **YAGNI (You Ain't Gonna Need It)**: Build only what's needed NOW
* **KISS (Keep It Simple, Stupid)**: Complexity is the enemy of maintainability
* **Less is More**: Prefer 10 lines that are clear over 100 that are clever
* **Code is Read 10x More Than Written**: Optimize for readability
* **Self-Documenting Code**: Code should explain itself; comments only for "why", not "what". Variable names should **ALWAYS** be clear and descriptive, even in inline map/filter functions.
* Use **pure functions by default**; introduce a class only for shared mutable state or real polymorphism.
* **Compose > Inherit** — build features by combining small functions/objects instead of subclass trees.
* Start with `interface` / `type`; add a class only when behaviour + state demand runtime instances.
* Flag any module>200 LOC or class>5 public methods as a “god object” to be split.
* Keep FP readable: short `map`/`filter` chains fine; avoid nested, point‑free puzzles.
