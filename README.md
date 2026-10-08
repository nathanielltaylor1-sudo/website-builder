# website-builder

## Writing skills

This repo ships the [humanizer-stack](https://github.com/NulightJens/humanizer-stack)
as project-level Claude Code skills, so they load automatically in any Claude Code
session opened here:

- `humanizer`: pass 1, words and phrasing
- `structural-humanizer`: pass 2, discourse structure

Run pass 1 first, then pass 2, on any site copy before publishing ("humanize this
page", "run the structural pass on hero.md"). See
[`third_party/humanizer-stack/PIPELINE.md`](third_party/humanizer-stack/PIPELINE.md).

The deterministic scanners can also be run on their own:

```bash
python3 .claude/skills/humanizer/scripts/copy_scan.py <file>
python3 .claude/skills/structural-humanizer/scripts/structural_scan.py <file>
# --json for machine-readable output, --strict to exit 1 on hits, --html to strip tags
```

Licensing and attribution: [`third_party/humanizer-stack/`](third_party/humanizer-stack/).
