# Interesting Decisions — Agent Skills

Three portable [Agent Skills](https://agentskills.io/specification) for game design, inspired by Sid Meier's talks and memoir. They turn a design idea into a small, testable change rather than a longer design document. For digital and tabletop games; no game engine or network access required.

| Skill | Use it for | Output |
| --- | --- | --- |
| [decision-design](skills/decision-design/SKILL.md) | Design or audit a mechanic, strategy, or turn | A decision table and one proposed change |
| [player-experience-review](skills/player-experience-review/SKILL.md) | Diagnose unfair-feeling odds, opaque losses, or a slow start | A failure trace and a testable fix |
| [playtest-iteration](skills/playtest-iteration/SKILL.md) | Plan or interpret the next prototype/playtest | A paired test and an evidence-based decision |

**Install in Codex:** copy the desired folders from `skills/` to your project's `.agents/skills/`. Open the project in Codex, then invoke a skill by name or describe the task. Other Agent Skills-compatible clients use their own skill directory. Supporting materials in `examples/` are optional.

**Try:** “Use `decision-design` to audit this turn. Show me two reachable states that favor different actions, or tell me why the same action wins in both.”

See the [worked example](examples/beacon-run.md) and [source notes](SOURCES.md). This is an independent adaptation, not an official Sid Meier, Firaxis, or GDC project.

## 日本語

シド・マイヤーの講演と回顧録から着想を得た、ゲーム開発向けのAIエージェントスキル集です。入力や回答は日本語でも使えます。

1. **選択肢の設計**：何を捨てて何を取るのか、どんな盤面なら答えが逆転するか。
2. **体験のレビュー**：先読みできたか、負けた理由が伝わったか、次に何を試せるか。
3. **プレイテスト**：ベースラインと変更案を比べ、測ったことと推測を分ける。

試すなら「このルールを `decision-design` で診断して。状況によって最善手が逆転するか、具体的な盤面を2つ出して」と頼んでください。
