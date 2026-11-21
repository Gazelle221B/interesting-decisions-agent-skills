# Worked example: Beacon Run

Original, fictitious two-player prototype. All results below are paper traces or test plans, not observed playtests.

**Rules.** You have two turns left and need 4 more points. Each turn choose **Scan** for 2 points, or **Relay** for 1 point and raise the shared signal by 1 (cap 3). A **charged relay** using signal 3 instead scores 4 and resets signal to 0. You go next in both states; your rival has one turn between yours and can only Scan in these two states (their relay is disabled).

- **Decision design:** At signal 0, two Scans reach 4; either two ordinary Relays or Relay + Scan falls short. At signal 3, charged Relay gets 4 now but drains the shared signal, while two Scans leave the signal alone and delay scoring. If the only goal is to reach 4 by the end and the rival cannot interact, both routes succeed in state 2; there is no forced tradeoff. In a third fixture, use final relative score instead: start at player 0, rival 1, and signal 3, with the rival's Relay enabled. A first Scan lets the rival take the charged Relay and reach 5; a first charged Relay denies that response and guarantees at least 5 for you versus at most 3 for the rival. The opponent's ability to act changes the best move; merely counting pick rates would miss why.
- **Experience review:** If a player tries Relay at signal 2 expecting 4, show “1 now → signal 3” versus “4 now → signal 0” in the preview. Keep the rule unchanged. Ask for a prediction before clicking and an explanation afterward.
- **Iteration:** A = current card text. B = explicit before/after preview. Present both signal states in counterbalanced order. Primary metric: correct prediction of points and resulting signal. Guardrail: no slower decisions beyond an agreed margin. Track each attempt and report how many participants saw each version; do not substitute simulation for understanding.

The rule text is the fixture. Ask the agent to enumerate two-turn outcomes, check the premise about the rival, or propose a second rival-enabled fixture before changing rewards.
