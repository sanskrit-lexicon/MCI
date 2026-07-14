# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**MCI** is the development and correction repository for **the *Mahābhārata Cultural Index* (A. D. Pusalker et al.)**, a specialized cultural and onomastic index to the Mahābhārata, within the [Cologne Digital Sanskrit Lexicon](https://www.sanskrit-lexicon.uni-koeln.de/) (CDSL).

- **Canonical source text**: [`csl-orig/v02/mci/mci.txt`](https://github.com/sanskrit-lexicon/csl-orig/blob/main/v02/mci/mci.txt) (2,325 index entries) — corrections are applied to that file, not stored here.
- This repository holds **development artifacts**: corrections, markup, comparison, and per-issue working files.
- A partial, still-growing index of names and cultural references in the Mahābhārata rather than a general dictionary.

## Key commands

Corrections follow the CDSL `updateByLine.py` pattern, applied against the csl-orig source:

```sh
python updateByLine.py <input> <changefile> <output>
```

Change-file format (paired lines; `;`-prefixed comments):

```
1234 old <original line>
1234 new <replacement line>
```
Supports `new` (replace), `ins` (insert after), `del` (delete). All files UTF-8 (**no BOM**).

## Data format

MCI entries use standard CDSL Sanskrit-lexicography markup. See [DATA_DICTIONARY.md](DATA_DICTIONARY.md) for the full tag reference.

| Tag | Role |
|---|---|
| `<L>NNNN<pc>PPP` | Entry begin, with print page-column ref |
| `<k1>`, `<k2>` | Primary / secondary headword (SLP1) |
| `<LEND>` | Entry end |
| `{#…#}` | Sanskrit text (SLP1) |
| `{%…%}` | English gloss / italic display text |
| `¦` | Headword / definition separator |
| `<lex>…</lex>` | Lexical category |
| `<ls>…</ls>` | Literary source citation |

Annotated example — the first entry of `mci.txt`:

```
%***This_File_is_MCI_AB(CORR5).TXT,_Last_update_26.08.13 L1555
;
; TITLE, volume 1, Fascicule 1
;
[Page00-01+ 10]
<H>{@MAHĀBHĀRATA—CULTURAL INDEX@}
Volume One
Fascicule |
EDITOR
M. A. MEHENDALE
Indolo
```

## Dependencies

- Python 3 (correction and comparison scripts).
- No build step in this repo; XML and web display are generated centrally from `csl-orig` via `csl-pywork`.

## GitHub Issue Conventions

This repository uses the Cologne dictionary-repo issue taxonomy. Every issue has exactly one **type**, one **severity**, and one **milestone**:

- **Type** (9): link-target, link-splitting, markup, text-correction, content-enhancement, encoding, scan-quality, bug, question
- **Severity** (3): minor, medium, hard
- **Milestone** (4): Dictionary to Book, Digitization Quality, Structured Data, Major Enhancements

See the [Cologne issue runbook](https://github.com/sanskrit-lexicon/csl-observatory/blob/main/runbook/cologne-issue-runbook.md) for label definitions and the type→milestone mapping.