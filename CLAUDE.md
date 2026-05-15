# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**MCI** is the corrections repository for the Cologne digitization of Sorensen's *Mahabharata Cultural Index*. The canonical source lives in `csl-orig/v02/mci/mci.txt`.

Issues and corrections are tracked via the [GitHub issue tracker](https://github.com/sanskrit-lexicon/MCI/issues).

## Common Commands

### Apply line-level corrections (standard pattern)
```bash
python updateByLine.py <input_file> <changein_file> <output_file>
```

### Rebuild and validate XML (from `csl-pywork/v02/`)
```bash
sh generate_dict.sh mci ../../MCIScan/2020
sh xmlchk_xampp.sh mci
```

## Dependencies

- **Python 3**
- **mci.txt** — in `$BASE/cologne/csl-orig/v02/mci/mci.txt`
