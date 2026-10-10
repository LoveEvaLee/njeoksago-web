# Onbam (온밤) — Balanced Dream Interpretation

*Onbam* means "a whole night" in Korean.

[English] · [한국어](README.md)

Write down your dream, and the app matches it against rules structured from traditional dream-interpretation literature, then returns one of five verdicts: **auspicious · ominous · mixed · neutral · withheld**.

**▶ Try it: https://loveevalee.github.io/onbam-web/** (Korean UI)

## What makes it different

- **No flattery.** When good and cautionary signs coexist, both are shown — the verdict is "mixed", not whichever sounds nicer.
- **Every verdict ships with its evidence** — which lineage of literature reads it that way, under which conditions, at what agreement score.
- **Thin evidence → no verdict.** Instead of forcing an answer, it withholds judgment and offers a symbol dictionary.
- **Deterministic.** The language layer only extracts symbols and scene facts; the verdict itself is computed by plain code, so the same dream always gets the same verdict. Scoring coefficients are public in `kb.json`.

## Repository layout

```
index.html    the whole app (single file — extraction + verdict engine)
kb.json       knowledge snapshot (symbols · rules · scoring)
assets/       intro motion graphic
docs/         how the verdict is computed (Korean)
```

Source data (literature cross-referencing workbench) and the collection pipeline live in a private repository; only built artifacts are published here.

Code is MIT-licensed; see [LICENSE](LICENSE) for a note on the interpretation data. This is a Phase 0 public trial. It presents readings from traditional literature — it does not predict the future, and it is not a substitute for counseling.
