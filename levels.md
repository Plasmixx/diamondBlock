# diamondBlock — Math Levels Spec (11/21/26)

**(mm/dd/yy format)**

Real app only. Replaces the landing-page 4-level Easy / Medium / Hard / Very Hard system for the app unlock. Level is picked at onboarding and stored locally on the device (no account, per the no-accounts proposal — see note at the bottom).

## Progression order (22 levels)

1. Pre-K
2. Kindergarten
3. 1st Grade
4. 2nd Grade
5. 3rd Grade
6. 4th Grade
7. 5th Grade
8. 6th Grade
9. 7th Grade
10. Algebra 1
11. Geometry
12. Algebra 2
13. Pre-Calculus
14. Differential Calculus
15. Integral Calculus
16. Multivariable Calculus
17. Linear Algebra
18. Discrete Math
19. Differential Equations
20. Real Analysis
21. Topology
22. Stochastic Calculus

## Warning prompts

### Too-Easy Warning — Pre-K, Kindergarten, 1st Grade
Triggered on selecting any of these three.
Text: "If you aren't actually at a 1st-grade math level or below, don't pick this. Remember: you downloaded diamondBlock to focus, not just to say you downloaded a focus app."
- Primary button: Pick a Higher Level
- Secondary option: Continue Anyway

### Hard Warning — Integral Calculus through Differential Equations
Triggered once on selecting Integral Calculus, Multivariable Calculus, Linear Algebra, Discrete Math, or Differential Equations.
Asks if they're sure. One confirmation prompt.

### Extreme Warning — Real Analysis, Topology, Stochastic Calculus
Triggered on selecting Real Analysis, Topology, or Stochastic Calculus.
This REPLACES the Hard Warning — it is 2 prompts total, not 3:
1. "Are you sure?"
2. "Are you absolutely sure you want to choose this?"
If they confirm the second one, the level saves.

## Level Change Cooldown (Settings)

- One free level change, in case the wrong level was picked at signup.
- After that one free change is used, the change button locks.
- It unlocks again after 7 days.
- Purpose: stop users dropping the difficulty down just to doomscroll.

## Notes / open problems

- Top levels (Real Analysis, Topology, Stochastic Calculus) are proof-heavy in real life. The app needs computational, auto-gradeable problems for them (e.g. compute, evaluate, find), not proofs — that problem design is still open.
- Cooldown is stored locally with the level. With no accounts / no server, deleting and reinstalling the app would reset it. That is the tradeoff of the no-accounts design; it stops casual difficulty-dropping, not a determined reinstall.
- Landing-page Solve simulation still uses the old 4 levels (Easy/Medium/Hard/Very Hard). That is a demo only and is not changed by this spec unless the user asks.
