# humanizer-stack (vendored)

Upstream: https://github.com/NulightJens/humanizer-stack
Pinned at commit `13f5c023189d428ffba726c75886ca1fd0dcba65`.

`LICENSE` and `ATTRIBUTION.md` are copied unmodified and travel with the vendored
files. `ATTRIBUTION.md` uses upstream paths; they map to this repo as follows:

| Upstream path | This repo |
|---|---|
| `skills/humanizer/**` | `.claude/skills/humanizer/**` |
| `scripts/copy_scan.py` | `.claude/skills/humanizer/scripts/copy_scan.py` |
| `skills/structural-humanizer/**` | `.claude/skills/structural-humanizer/**` |
| `docs/PIPELINE.md` | `third_party/humanizer-stack/PIPELINE.md` |

Local changes: scanner and pipeline paths in `SKILL.md`, `copy-tells.md`, and
`PIPELINE.md` were rewritten to match the layout above. Nothing else was changed.

To update, re-copy from upstream and re-apply the path edits.
