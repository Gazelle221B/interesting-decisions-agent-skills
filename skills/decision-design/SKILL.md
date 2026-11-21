---
name: decision-design
description: Design or review meaningful player choices in video games or tabletop games. Use for game mechanics, combat actions, resource tradeoffs, progression paths, dominant strategies, or a turn that feels automatic. Not for engine implementation or formal game-theory proofs.
---

# Design a meaningful decision

Reply in the user's language. Keep the requested theme, audience, non-negotiable rules and production scope. If a missing rule prevents analysis, label the assumption or ask for that rule. Never quietly add a resource or win condition.

1. Select one consequential decision. State the player's objective, timing, legal actions (including waiting), observable information, and what the player cannot know. Use player-visible information, not engine hindsight.
2. Trace alternatives in at least two concrete reachable states when feasible. For each, state an immediate gain, what is given up, any relevant delayed effect or counterplay, and the expected feedback. Include a different player goal/style only if it changes a consequence.
3. Diagnose the actual failure:
   - **Dominance:** one choice is never worse and sometimes better over the stated scope; two samples suggest dominance but do not prove it globally.
   - **No effect:** different buttons produce effectively interchangeable consequences for the player's goal.
   - **Unreadable:** a real difference exists but players cannot infer its direction or stakes.
   - **Overload:** the choice costs attention without a worthwhile payoff. It may be better to combine or remove options.
4. Propose one small change to the strongest issue. Fix unreadability with information before adding complexity. For dominance, look for a contextual cost, timing conflict or counterplay; not every option needs equal usage, and equal pick rates can reflect guessing rather than thought. Keep uncertainty where the player can still choose how much risk to take.
5. Replay the same states under the change, including a trivial exploit or degenerate policy if one is plausible. State a falsifiable playtest question. Don't claim that paper analysis proves fun.

## Output

Return a decision table (state / what the player sees / choices / costs and effects / current best choice or tradeoff), then the main finding, one change and the smallest experiment that could overturn it. Separate facts from assumptions. If there is no explicit decision to improve, preserve the rhythm, exploration or execution challenge rather than forcing arbitrary branches.
