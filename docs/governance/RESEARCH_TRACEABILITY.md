# Research traceability and validation / 研究トレーサビリティ・検証計画

**GL-RTM-001 v0.1 · 2026-11-26 JST · Proposed / 計画**

[Market evidence / 市場証拠](../market-research/MARKET_EVIDENCE.md) · [Portfolio](../../README.md)

This is a portfolio-level index, not a replacement for repository SRS/DVP/DVR. MP IDs describe provisional market problems; VR IDs below are proposed user-value studies. Existing requirement IDs retain their original namespace and meaning. No market study is marked PASS from a technical test.

| MP | Existing specification / 既存要件 | Technical evidence / 技術証拠 | Proposed study / 効果検証 | Status |
|---|---|---|---|---|
| MP-05 | [VOCALOID R03/R04/R09; T03–06](https://github.com/Gacky-Lab/AI-VOCALOID-STUDIO/blob/main/docs/design.md), [MIR-07/08](https://github.com/Gacky-Lab/AI-MUSIC-INTELLIGENCE-ENGINE/blob/main/docs/requirements.md), [Optimizer FR-18](https://github.com/Gacky-Lab/SUNO-GENERATION-OPTIMIZER/blob/main/docs/requirements.md) | Offline score interfaces; synthetic note candidates; native asa draft PoC is owner-reported, not a verified preservation test | VR-05: short lyric/expressive edit with explicitly preserved targets | NOT_RUN |
| MP-02 | [SGO FR-08/12/13/14/15/17](https://github.com/Gacky-Lab/SUNO-GENERATION-OPTIMIZER/blob/main/docs/requirements.md) | [P2 repeated DVR](https://github.com/Gacky-Lab/SUNO-GENERATION-OPTIMIZER/blob/main/docs/P2_REPLICATED_DVR.md): tested intervention did not show advantage; P1 real-audio measurements limited | VR-02: matched budget and requirements, independent acceptance and actual time/cost | NOT_RUN for user-value endpoint |
| MP-04 | [CDE v0.1](https://github.com/Gacky-Lab/AI-MUSIC-INTELLIGENCE-ENGINE/tree/main/research/creative-deviation-evaluation) | Proposal and observation protocol only | VR-04: restoration preference and delayed choice; separate future reuse comparison | NOT_RUN |
| MP-03 | [MIR-07](https://github.com/Gacky-Lab/AI-MUSIC-INTELLIGENCE-ENGINE/blob/main/docs/requirements.md), [VOCALOID T03/T04](https://github.com/Gacky-Lab/AI-VOCALOID-STUDIO/blob/main/docs/design.md) | [Review-only note candidates](https://github.com/Gacky-Lab/AI-MUSIC-INTELLIGENCE-ENGINE/blob/main/docs/NOTE_CANDIDATES.md); synthetic accuracy only | VR-03: annotated audio note accuracy and correction time | NOT_RUN |
| MP-06 | [AMVS R01/R02/R04/R05/R07/R08/R12](https://github.com/Gacky-Lab/AI-MUSIC-VIDEO-STUDIO/blob/main/docs/requirements.md) | [Synthetic integration](https://github.com/Gacky-Lab/AI-MUSIC-VIDEO-STUDIO/blob/main/docs/FIVE_REPO_INTEGRATION.md), 30s render | VR-06: human-reviewed authorized lyric MV compared to existing manual workflow | NOT_RUN |
| MP-01 | [Lyric validation §§1–7](https://github.com/Gacky-Lab/LYRIC-DESIGN-FRAMEWORK/blob/main/docs/validation.md) (section reference, no fabricated requirement ID) | [Study preflight](https://github.com/Gacky-Lab/LYRIC-DESIGN-FRAMEWORK/blob/main/docs/STUDY_SELECTION_AND_EVIDENCE.md), listener data NOT_RUN | VR-01: revision effort and author assessment, controlled comparison | NOT_RUN |

## First study / 最初の検証 VR-05

- Start with original short, authored MIDI and lyrics; licensed/authorized singing environment. No paid generation or external media transfer is authorized by this plan.
- Before editing, register creator, intended change, preserved target, permitted changes, input identity, tolerance and comparator. Use a manual edit or supported existing tool as baseline, and the proposed assisted workflow as candidate. Match source, task and permitted work; log failures and manual intervention.
- Measure target-specific note alignment and errors (pitch, onset, duration with predefined tolerances), intended lyric correctness and elapsed active edit/review time. Record whether the result is acceptable to the creator independently of technical checks. Do not reduce artistic acceptance to a signal metric.
- Prespecify how edits affecting syllable count or pronunciation will be handled; if other factors cannot be controlled, mark COMPOSITE and report separately. A constructed deviation is SIMULATED, not an observed AI failure.
- Start with a single-creator exploratory feasibility pilot; sample size, smallest worthwhile difference and analysis for later confirmation require prospective justification. Report uncertainty, missing cases, ties, exclusions and negative results; no arbitrary success threshold is validated yet.
- Go to a larger study only if the comparator and proposed workflow are both executable, evidence and permissions are complete, and the pilot demonstrates a feasible comparison. Otherwise revise or stop.

日本語：短い自作素材で、変更対象・保持対象・比較手段を事前に固定する。歌詞の正しさ、音符差、修正時間、本人の採否を別々に測る。比較不能・欠測・失敗も残す。実験計画の成立とユーザー価値の実証は別。

## Other study endpoints / その他の効果指標

| Study | Proposed endpoint | Boundary |
|---|---|---|
| VR-02 | Credits/time per creator-accepted result, plus success proportion within equal budget | Zero accepted candidates: ratio undefined; report spend and failures. Provider BPM is not independent acceptance. |
| VR-03 | Note precision/recall with prespecified matching, correction minutes | Use annotated reference; report unsupported polyphony and failed tracks. |
| VR-04 | Off-diagonal CDE fraction, repeated decisive preferences; separate held-out reuse task | No inference of psychology or reuse from classification alone. |
| VR-06 | Active edit time, timing error against annotated anchors, human review | Report render failures and artistic judgement separately. |
| VR-01 | Revision time and author preference; separately controlled text or audio task | No hit prediction; no single-factor attribution from composite audio. |

## Status and risk / 状態・リスク

- Technical PASS is scoped to the cited tests and pinned commits. Do not retag historical integration runs or claim CDE was executed in them.
- Market demand, real-song preservation, full vocal production, CDE listening, independent replication and actual savings are unvalidated.
- Research and production rights differ. Review [provider terms](https://suno.com/terms), voicebank and tool licenses before each external use; default to original/authorized fixtures, offline. No redistribution of private music, proprietary assets, signed URLs or participant records.
- Public visibility is not a reuse license. License selection is a maintainer decision; do not introduce a blanket license without explicit approval. See each repository's notices.
- Preserve baseline specifications and negative results. Any changed priorities or test acceptance criteria require a dated rationale. 

Status labels: PROPOSED / NOT_RUN / BLOCKED / PARTIAL / PASS / FAIL / UNKNOWN. A PASS always requires a scope, evidence link and date. Do not infer user benefit or market demand from a design or CI pass.
