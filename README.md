# Nikit Kashyap

**KYNEX** — a local, tool-using AI agent that extracts structured data from documents.

<p align="center">
  <a href="https://github.com/Nikit117/kynex-harness">
    <img src="https://img.shields.io/badge/KYNEX-92.65%20unified%20value%20F1%20on%20ExtractBench-3b82f6?style=flat-square" alt="ExtractBench">
  </a>
  <img src="https://img.shields.io/badge/ExtractBench-rank%2012%2F50-38bdf8?style=flat-square" alt="rank">
  <img src="https://img.shields.io/badge/python-3.11%2B-3b82f6?style=flat-square" alt="python">
  <img src="https://img.shields.io/badge/license-Apache--2.0-3b82f6?style=flat-square" alt="license">
</p>

### What I build

A tool-using extraction agent for documents: it stages a PDF, calls tools against
it (page text, tables, layout analysis, rendered pages) and returns JSON that
validates against your schema — plus the five post-processing rules that the
measurements showed were needed.

| | |
|---|---|
| **92.65** unified value F1 on [ExtractBench](https://github.com/run-llama/ExtractBench) (370 documents, unmodified official scorer) — **rank 12 of 50** | [leaderboard PR](https://github.com/run-llama/ExtractBench/pull/84) |
| **14.29 ¢** per page, 190 k input tokens per document | [docs/benchmarks.md](https://github.com/Nikit117/kynex-harness/blob/main/docs/benchmarks.md) |
| Interactive TUI, scriptable CLI, and an ExtractBench provider | [docs/usage.md](https://github.com/Nikit117/kynex-harness/blob/main/docs/usage.md) |

<p align="center">
  <a href="https://github.com/Nikit117/kynex-harness">
    <img src="https://img.shields.io/github/stars/Nikit117/kynex-harness?style=social" alt="stars">
  </a>
</p>

```bash
git clone https://github.com/Nikit117/kynex-harness
cd kynex-harness && pip install -r requirements.txt
python -m autonomous_document_harness.tui
```

<p align="center"><sub>Extraction is the easy part. Knowing <i>which</i> rows are records is the hard part.</sub></p>
