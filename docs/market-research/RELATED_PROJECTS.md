# Related projects and alternatives / 既存手段・関連研究

**GL-COMP-001 v0.1 · 2026-11-26 JST · Public-source comparison**

This is a selected comparison, not an exhaustive competitive landscape, performance benchmark or claim of superiority. Repository descriptions and documentation were reviewed; competitors' code was not executed. Related projects may be collaborators or dependencies as well as alternatives.

| Project | Existing capability / 既存価値 | Implication for Gacky-Lab / 研究方針 |
|---|---|---|
| [Claude AI Music Skills](https://github.com/bitwize-music-studio/claude-ai-music-skills) | End-to-end human+AI workflow, lyrics, audio mastering, release tooling, documented CI and skills | Closest workflow comparison. Integration, quality gates and prompt guidance alone are not unique. Focus on controlled evidence of preservation and creator choices. |
| [music_studio](https://github.com/meicale/music_studio) | Local AI generation, stems, DAW, MIDI and arranger | Avoid rebuilding general DAW/generation functions unless comparative need is shown. |
| [suno-band-manager](https://github.com/zarlor/suno-band-manager) | Prompt/lyric validation, cliché and syllable checks, structured song packages | Lyric structure and validation are established; test the specific editorial workflow rather than claiming novelty. |
| [SunoMCP](https://github.com/AceDataCloud/SunoMCP) · [suno-mcp-server](https://github.com/frankxai/suno-mcp-server) | Third-party generation connector or prompt-strategy tools | Connection alone is not a differentiator. Prefer authorized interfaces and bounded experiments. |
| [MuseCPEval](https://github.com/Yashvishe13/MuseCPEval) · [MuseCPBench](https://arxiv.org/abs/2512.14629) · [SMEBench](https://arxiv.org/abs/2610.36715) | Musical-context preservation metrics and controlled symbolic editing benchmarks | Do not duplicate established metrics or claim restoration alone is new. CDE studies whole-artifact adoption vs target-level choice; empirical novelty remains unverified. |
| [ACE-Step](https://github.com/ace-step/ACE-Step) · [YuE](https://github.com/multimodal-art-projection/YuE) | Music generation model and editing capabilities | Model development is not the current focus. Consider only appropriate permitted baselines. |
| [Basic Pitch](https://github.com/spotify/basic-pitch) | Audio-to-MIDI transcription | Use as a possible licensed benchmark; no claim that current MIR candidates outperform it. |
| [OpenUtau](https://github.com/openutau/OpenUtau) | Singing synthesis editing platform | Existing editable score/singing workflows; investigate interoperability and preservation rather than recreating editors. |
| [TextAlive App API](https://github.com/TextAliveJp/textalive-app-api) | Music-synchronized lyric apps | Existing lyric timing and visualization; distinguish rendered production and version/approval traceability. |
| [Suno Song Editor](https://help.suno.com/en/articles/6141505) · [MIDI in Studio](https://help.suno.com/en/articles/13670593) · [Sample/Mashup](https://suno.com/release-notes/meet-our-new-create-features-sample-mashup) | Official editing, MIDI and recombination | Treat current features as baselines, not unmet needs. Recheck capabilities before each study. |

## Positioning / 差別化の仮説

The portfolio's intended contribution is a traceable link from creative intent through edit and measured evidence to human judgement and possible reuse, not a claim that all its components are original. Its advantage over current production tools remains to be established by controlled studies.

創作意図→変更→音楽的証拠→人間の判断→再利用仮説を追跡することに注力する。機能数や統合そのものを新規性とせず、比較で差が出ない機能は縮小する。第三者コードのライセンスやサービス規約は個別に確認し、本表は利用許諾を意味しない。
