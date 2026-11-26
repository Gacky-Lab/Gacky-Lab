# Market evidence and problem hypotheses / 市場課題・証拠台帳

**GL-MKT-001 v0.1 · 2026-11-26 JST · Exploratory / 探索的調査**

[Portfolio / 全体方針](../../README.md) · [Requirements and validation / 要求・検証](../governance/RESEARCH_TRACEABILITY.md) · [Related projects / 既存手段](RELATED_PROJECTS.md)

## Scope / 調査範囲

Primary hypothesis: independent creators who generate music and subsequently want to control specific lyrics, melody, singing or arrangement. Secondary audience: music technology developers and co-creation researchers. The research starts from creator experience and purposive public-source observation, not a representative survey.

主対象はAI生成後に歌詞・旋律・歌唱・編曲を細かく修正する個人制作者。副対象は音楽技術開発者・共創研究者。以下は課題別に検索した公開資料の探索的な標本であり、母集団・発生率・支払意思は測定していない。投稿者の属性・独立性・利用環境は未確認。同一話題の再投稿やベンダー投稿を独立ユーザー数として数えない。

Search terms / 検索語: Suno change lyrics keep melody/voice; wasted credits; MIDI export inaccurate; combine favorite parts of generations; music video editing time; generic AI lyrics; PAGURI. Search date / 調査日: 2026-11-26 JST. Public evidence below is paraphrased; no usernames or private media collected. Search selection is convenience-based and may overrepresent complaints.

## Evidence register / 証拠台帳

Source type: U = public user report (unverified self-report); P = official feature documentation or provider announcement; R = research. Evidence IDs are references, not validated customer requirements.

| ID | MP | Type | Source | Observation and limitation / 観測・限界 |
|---|---|---|---|---|
| E01 | 05 | U | [Keep voice when modifying lyrics](https://www.reddit.com/r/SunoAI/comments/1t1y4zb/how_the_hell_do_i_get_it_to_keep_the_voice_when/) | One user reports difficulty keeping voice while changing a verse; replies suggest aligning pacing and editing vocal stems. / 歌唱保持の困難と回避策。 |
| E02 | 05 | U | [Change text without changing notes](https://www.reddit.com/r/SunoAI/comments/1rmr4tm/is_it_actually_possible_to_make_it_change_the/) | User reports notes/timbre changing; replies describe alternative workflows. / 音符・声質の変化。 |
| E03 | 05 | U | [Minor lyric edits workflow](https://www.reddit.com/r/SunoAI/comments/1wnj1ql/if_you_need_to_make_some_minor_changes_to_lyrics/) | Counterexample: a user reports a method that largely retains original arrangement, melody and vocal take. / 既存手段で改善できた例。 |
| E04 | 05 | P | [Song Editor](https://help.suno.com/en/articles/6141505) · [Replace Section](https://help.suno.com/en/articles/3271873) | Local regeneration and lyrics editing exist; this does not establish exact retention or its absence across all modes. / 部分編集は既存機能。 |
| E05 | 02 | U | [Generation credits and instruction following](https://www.reddit.com/r/SunoAI/comments/1wt82m2/suno_v6_is_becoming_difficult_to_justify/) | Reported time/credit burden; not independently measured. / 再生成の負担。 |
| E06 | 02 | U | [Quality and repeated generation](https://www.reddit.com/r/SunoAI/comments/1xyot8d/suno_is_going_backward_fix_music_generation_false/) | November 17, 2026 self-report of repeated generations due to perceived defects. / 不具合を理由とする再生成。 |
| E07 | 02 | U | [Credit discussion](https://www.reddit.com/r/SunoAI/comments/1wg6h4h/sunos_credit_math_is_messed_up/) | Positive experience with improved output also appears; not every user faces the same burden. / 改善を報告する例もある。 |
| E08 | 03 | U | [MIDI export and DAW import](https://www.reddit.com/r/SunoAI/comments/1rdj411/exporting_midi_files_are_totally_not_alike_the/) | User reports exported notes not matching perceived song. No ground-truth score or error rate. / MIDI精度への不満。 |
| E09 | 03 | P | [MIDI in Studio](https://help.suno.com/en/articles/13670593) · [MIDI improvement announcement](https://www.reddit.com/r/SunoAI/comments/1wiyua5/midi_just_got_better_in_suno_studio/) | Existing piano-roll editing and reported provider improvements; not independent benchmarks. / 現行機能と改良。 |
| E10 | 04 | U | [Combining favorite parts](https://www.reddit.com/r/SunoAI/comments/1sij6ue/how_do_you_combine_the_best_parts_of_multiple/) | User wants to combine liked portions across versions. This supports a related workflow need, not demand for CDE specifically. / 複数候補の魅力を活用したい声。 |
| E11 | 04 | U | [Selecting best parts of generations](https://www.reddit.com/r/SunoAI/comments/1vilv0m/let_us_select_the_best_parts_from_multiple/) | User proposes selection of favored musical portions; overlap with existing editing features. / 選択した要素の保持要望。 |
| E12 | 04 | P/U | [Sample + Mashup](https://suno.com/release-notes/meet-our-new-create-features-sample-mashup) · [Successful Studio combination report](https://www.reddit.com/r/SunoAI/comments/1mx60rj) | Existing recombination and user-reported success; CDE is not a recombination algorithm. / 組合せ機能・成功例が存在。 |
| E13 | 06 | U | [Music video workflows](https://www.reddit.com/r/SunoAI/comments/1y4wd05/how_are_you_making_videos_for_your_suno_songs/) | Reports of time spent assembling short clips into videos; other users have custom workflows. / 映像の手作業と代替策。 |
| E14 | 06 | U | [Video tooling comparison](https://www.reddit.com/r/AI_Music/comments/1y3l7aw/which_ai_music_video_tool_would_you_actually_keep/) | Discussion of differing tools and edit effort; individual experience only. / ツール別の修正負担。 |
| E15 | 01 | U | [Repeated generated lyric phrases](https://www.reddit.com/r/SunoAI/comments/1dhh61w/list_of_overly_used_phrases_in_the_generated/) | Complaint about repeated phrases; a reply uses own lyrics. Does not establish need for a specific scoring rubric. / 定型表現と自作による回避。 |
| E16 | 02,05 | R | [PAGURI: A User Experience Study of Creative Interaction with Text-to-Music Models (2025)](https://www.mdpi.com/2079-9292/14/17/3379) | User-experience research on interactions with text-to-music generation; not a Gacky-Lab demand survey. / 生成音楽の利用体験研究。 |
| E17 | 04,05 | R | [MuseCPBench](https://arxiv.org/abs/2512.14629) · [SMEBench](https://arxiv.org/abs/2610.36715) | Related preservation metrics and controlled editing benchmarks. Research evidence, not proof of market size or CDE novelty. / 関連評価・統制編集研究。 |

## Problem map / 課題の優先順位

| MP | Problem / 課題 | Evidence | Decision / 判断 | Evidence gap / 未確認 |
|---|---|---|---|---|
| 05 | Preserve desired expressions during edits / 表現保持 | E01–04,E16–17 | P1: first controlled comparison | Actual edit burden and comparison with current tools |
| 02 | Repeated generation effort / 再生成負担 | E05–07,E16 | P1: bounded comparison | Time, credit cost per accepted output, negative results |
| 04 | Overlooked creative changes / 創作価値の見落とし | E10–12,E17 | P2: exploratory CDE research | Specific demand and restoration-comparison usefulness |
| 03 | Note correction / 音符修正 | E08–09 | P2: support MP-05 | Annotated real-song errors and manual correction time |
| 06 | Video production effort / MV負担 | E13–14 | P3: retain, defer expansion | User time compared with existing video tools |
| 01 | Lyric revision decisions / 作詞判断 | E15 | P3: retain, defer expansion | Need for rubric and actual revision benefit |

P1–P3 here are portfolio priorities, not the implementation phase names in individual repositories. No scores imply market share or customer acceptance. Review the priorities after interviews and comparative trials. No evidence for demand is not evidence of no demand.

## Next evidence / 次の市場検証

Conduct 5–8 exploratory, consenting creator interviews as a starting target (not a representative sample). Recruit creators who recently edited a generated song; include people satisfied with existing tools and those who abandon or avoid editing. Ask about their last actual edit, intended change, preserved elements, tools, time/cost, outcome and workarounds before presenting any proposed solution. Record counterexamples; do not collect private recordings or identifiers in public Git. Follow with the comparison plan in the traceability document.

利用者調査は未実施。既存製品の機能、規約、ユーザーの回避策が変化した場合は再評価し、不要な機能の開発を中止・縮小する。市場規模・購入意向・課題発生率は別途検証が必要。
