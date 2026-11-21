---
name: playtest-iteration
description: Plan, run within the available environment, or interpret small gameplay prototype experiments. Use for tuning a specific design hypothesis, comparing a baseline and variant, simulated balance checks, or deciding whether to keep, revise, or revert a mechanic.
---

# Make the next test informative

Reply in the user's language. Preserve the original rules/build and record assumptions. If you cannot run the game or recruit testers, deliver a runnable protocol or paper trace; do not describe it as a completed test.

1. Frame a falsifiable claim about one mechanic and a plausible competing explanation. Choose a baseline, a single reversible variant, and a primary observable. State what should improve, what must not degrade, and what result would make you revert.
2. Hold scenario, rules and policy constant except for the intended change. Use representative reachable states plus an edge case. When feasible, match scenario seeds for balance comparisons and record whether changed code alters random draws. Counterbalance A/B order with people when practice or memory can sway results.
3. If the direction is unclear, try one deliberately larger but reversible perturbation within safe bounds (or paper-test it) before fine tuning. For odds or tradeoffs, check extremes and simple exploit policies. Avoid compounding multiple changes.
4. Report the evidence type precisely:
   - **Paper trace:** feasibility and counterexamples under stated assumptions.
   - **Simulation:** rates under the modeled rules, seeds and bot policies. Report denominators and uncertainty where useful; no claims about human fun.
   - **Observed human play:** behavior and self-reports with counts, context and limitations. Do not overgeneralize from a small convenience sample.
5. Decide **keep / revise / revert / inconclusive** against your criteria. Record actual evidence, the main limitation and the next discriminating test. If nothing ran, mark the decision pending.

Return a compact test card: hypothesis, baseline/variant, controls, metric and guardrail, result by evidence type, and decision. One clean comparison beats several unrelated tweaks.
