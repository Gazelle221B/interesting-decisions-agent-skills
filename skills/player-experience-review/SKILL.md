---
name: player-experience-review
description: Review whether players can understand and act on what happens in a game. Use for onboarding, opaque losses, unfair-feeling randomness, boss difficulty spikes, feedback, pacing, or loss of agency. Distinguishes player perception from measured rules and observed behavior.
---

# Review the player experience

Reply in the user's language. Work from a build, rules, logs, screenshots or a concrete play sequence. Say what is missing instead of claiming how players felt.

1. Select one point where a player may lose control or confidence. Reconstruct **what was visible → what the player could reasonably predict → available response → actual outcome → what the game explained → next useful action**. For onboarding, find the first authentic core decision rather than imposing a fixed number of minutes.
2. Classify the failure: warning arrived too late, rule/odds were misread, counterplay was unavailable, feedback failed to name the cause, or the intended challenge itself was too hard. Separate no agency from the player knowingly taking a risk. Preserve suspense and genre-appropriate setbacks. For a side activity, check whether it reinforces the core loop or makes the player lose track of the main goal.
3. For randomness, distinguish an advertised probability, its implementation and sample rate, and what a player understands it to mean. Check whether a displayed ratio is a stat or literal odds. Account for repeated attempts, conditioning, dependence and small samples where relevant. Do not silently rig stated odds or infer unfairness from a single streak.
4. Change the least invasive layer first: timing and label, cause feedback, safe rehearsal, then mechanical tuning if evidence warrants it. Protect intended tension. Pick one fix and say which symptom it should change.
5. Test understanding separately from success. Before the outcome, ask testers to predict stakes without coaching; afterward, ask what happened and what they would do differently. Log their actual choices. High clear rates do not prove comprehension and bots cannot report felt fairness.

Return a failure trace, the strongest competing explanation, one proposed fix, and what evidence would distinguish the explanations.
