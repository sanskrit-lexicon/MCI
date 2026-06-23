# MCI front matter — OCR + translations

Faithful OCR of the **front matter** (title pages, editorial staff, foreword, editor's preface, and per-fascicule contents) of the **Mahābhārata Cultural Index** (MCI), with a Russian translation of every page and consolidated single-file editions.

## What this is

- **Dictionary:** *Mahābhārata — Cultural Index* — a comprehensive subject-wise index to the cultural information available in the *Critically Constituted Text of the Mahābhārata* published by the Bhandarkar Oriental Research Institute (BORI).
- **Editor:** M. A. Mehendale (Madhukar Anant Mehendale).
- **Publisher:** Bhandarkar Oriental Research Institute, Poona / Pune (India).
- **Span:** Vol. 1 (Fasc. 1–4, 1993–1997) and Vol. 2 (Fasc. 1–4, 1999–2007). The front matter proper (Foreword by R. N. Dandekar + Editor's Preface, signed M. A. Mehendale, 25 May 1993) appears in Vol. 1 Fasc. 1; the remaining pages are per-fascicule title pages and contents.
- **Source language:** **English** (Sanskrit headwords/terms in IAST and the occasional German imprint line are kept verbatim). Because the source is English, there is **no `.en.md`** — the base `.md` files are already English; only `.ru.md` translations are added.
- **Cologne source:** [mcipref.html](https://sanskrit-lexicon.uni-koeln.de/scans/csldev/csldoc/build/dictionaries/prefaces/mcipref.html) — 28 scans.

## File conventions

| Suffix | Meaning |
|---|---|
| `mciprefNN.md` | Page NN, faithful OCR in the source language (English). |
| `mciprefNN.ru.md` | Russian translation of page NN. |
| `scans/mci_0000-XX.jpg` | The source scan for each page (`.jpg`, 2128×2716 px for Vol. 1, 2484×2775 px for Vol. 2). |

Digitizer/library stamps (the Bonn *Indologisches Seminar* and Heidelberg *Südasien-Institut* inventory marks, handwritten inventory numbers, running headers/footers) are **omitted** as not part of the original.

## Consolidated editions

| File | Description |
|---|---|
| [mcipref_all.en.md](mcipref_all.en.md) | All 28 pages in order, English source, with a table of contents. |
| [mcipref_all.ru.md](mcipref_all.ru.md) | All 28 pages in order, Russian, with a table of contents. |
| [build_combined.py](build_combined.py) | Reproducible builder: `DICT=mci python build_combined.py`. |

## Contents (per page)

| NN | Section | Vol. | Source scan | RU |
|---|---|---|---|---|
| 01 | Title, Fasc. 1 (1993) | 1 | [mcipref01.md](mcipref01.md) | [ru](mcipref01.ru.md) |
| 02 | Title / sub-title, Fasc. 1 | 1 | [mcipref02.md](mcipref02.md) | [ru](mcipref02.ru.md) |
| 03 | Editorial Staff | 1 | [mcipref03.md](mcipref03.md) | [ru](mcipref03.ru.md) |
| 04 | Contents (Fasc. 1) | 1 | [mcipref04.md](mcipref04.md) | [ru](mcipref04.ru.md) |
| 05 | Foreword, 1 | 1 | [mcipref05.md](mcipref05.md) | [ru](mcipref05.ru.md) |
| 06 | Foreword, 2 (signed R. N. Dandekar, 25 May 1993) | 1 | [mcipref06.md](mcipref06.md) | [ru](mcipref06.ru.md) |
| 07 | Preface, 1 | 1 | [mcipref07.md](mcipref07.md) | [ru](mcipref07.ru.md) |
| 08 | Preface, 2 | 1 | [mcipref08.md](mcipref08.md) | [ru](mcipref08.ru.md) |
| 09 | Preface, 3 | 1 | [mcipref09.md](mcipref09.md) | [ru](mcipref09.ru.md) |
| 10 | Preface, 4 | 1 | [mcipref10.md](mcipref10.md) | [ru](mcipref10.ru.md) |
| 11 | Preface, 5 | 1 | [mcipref11.md](mcipref11.md) | [ru](mcipref11.ru.md) |
| 12 | Preface, 6 | 1 | [mcipref12.md](mcipref12.md) | [ru](mcipref12.ru.md) |
| 13 | Preface, 7 | 1 | [mcipref13.md](mcipref13.md) | [ru](mcipref13.ru.md) |
| 14 | Preface, 8 (signed M. A. Mehendale) | 1 | [mcipref14.md](mcipref14.md) | [ru](mcipref14.ru.md) |
| 15 | Title, Fasc. 2 (1995) | 1 | [mcipref15.md](mcipref15.md) | [ru](mcipref15.ru.md) |
| 16 | Contents (Fasc. 2) | 1 | [mcipref16.md](mcipref16.md) | [ru](mcipref16.ru.md) |
| 17 | Title, Fasc. 3 (1996) | 1 | [mcipref17.md](mcipref17.md) | [ru](mcipref17.ru.md) |
| 18 | Contents (Fasc. 3) | 1 | [mcipref18.md](mcipref18.md) | [ru](mcipref18.ru.md) |
| 19 | Title, Fasc. 4 (1997) | 1 | [mcipref19.md](mcipref19.md) | [ru](mcipref19.ru.md) |
| 20 | Contents (Fasc. 4) | 1 | [mcipref20.md](mcipref20.md) | [ru](mcipref20.ru.md) |
| 21 | Title, Vol. 2 Fasc. 1 (1999) | 2 | [mcipref21.md](mcipref21.md) | [ru](mcipref21.ru.md) |
| 22 | Contents (Vol. 2 Fasc. 1) | 2 | [mcipref22.md](mcipref22.md) | [ru](mcipref22.ru.md) |
| 23 | Title, Vol. 2 Fasc. 2 (2002) | 2 | [mcipref23.md](mcipref23.md) | [ru](mcipref23.ru.md) |
| 24 | Contents (Vol. 2 Fasc. 2) | 2 | [mcipref24.md](mcipref24.md) | [ru](mcipref24.ru.md) |
| 25 | Title, Vol. 2 Fasc. 3 (2004) | 2 | [mcipref25.md](mcipref25.md) | [ru](mcipref25.ru.md) |
| 26 | Contents (Vol. 2 Fasc. 3) | 2 | [mcipref26.md](mcipref26.md) | [ru](mcipref26.ru.md) |
| 27 | Title, Vol. 2 Fasc. 4 (2007) | 2 | [mcipref27.md](mcipref27.md) | [ru](mcipref27.ru.md) |
| 28 | Contents (Vol. 2 Fasc. 4) | 2 | [mcipref28.md](mcipref28.md) | [ru](mcipref28.ru.md) |

## Signatures / dates found

- **Foreword** (p. vii) — Bhandarkar Oriental Research Institute, Poona, India, **25 May 1993**, signed **R. N. Dandekar**.
- **Preface** (p. VIII) — signed **M. A. Mehendale** (no date; the Preface narrative runs to 1992).

Produced by the `/cologne-preface-ocr` skill (vision OCR + translation). See the root [README.md](../README.md) for run notes.
