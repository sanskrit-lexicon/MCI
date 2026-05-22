### Location

Counterpart of https://github.com/sanskrit-lexicon/PWG/issues/175 (PWG) and https://github.com/sanskrit-lexicon/PWK/issues/113 (PWK) for `mci.txt`.

I ran the same two-job recipe over `csl-orig/v02/mci/mci.txt`: auto-fix the few things with a single safe resolution; audit everything else with line refs. Added `08_markup_fix.py` plus outputs to a new `mciissues/markup_fix/` folder on the branch `markup-fix-audit`.

@funderburkjim @Andhrabharati — please review the findings listed below.

## Markup fixer + audit for `mci.txt`

### What it auto-fixes

| Pattern | Result |
|---|---|
| `<ab><ab>X</ab> Y</ab>` | `<ab>X Y</ab>` |
| `<sup> word </sup>` | `<sup>word</sup>` |
| `<F> word </F>` | `<F>word</F>` |

Whitespace trimming applies to all 2 paired tag(s) in `mci.txt`: `<sup>`, `<F>`. The original file is never modified — output goes to `mci_fixed.txt`, with the full diff in `markup_fix_changes.txt` (updateByLine format). **Output is byte-identical to source** (no auto-fixes triggered).

### Closing-tag inventory in current `mci.txt`

| Tag | Count |
|---|---:|
| `</sup>` | 806 |
| `</F>` | 21 |

### What it found in current `mci.txt`

- 0 whitespace trims — byte-identical to source.
- 0 adjacent `</ab> <ab>` — no `<ab>` tag in mci.txt.
- 0 `<ab n="…">` attributes.
- 135 `{{old → new || …}}` correction records present.

### Usage

```
cd mciissues/markup_fix
python 08_markup_fix.py                        # uses csl-orig/v02/mci/mci.txt by default
python 08_markup_fix.py IN.txt OUT.txt         # custom paths
```

Outputs: `mci_fixed.txt`, `markup_fix_changes.txt`, `markup_audit.txt`.

### Summary

Completely clean. Only <sup> and <F> paired tags.

### Severity

`minor`
