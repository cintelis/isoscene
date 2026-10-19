# isoscene

Polished isometric scenes as self-contained SVG, written from short Python scripts. No
dependencies beyond Python 3.10+; previews use a local Edge or Chrome.

It drew the scenes on sigilant.io and the case-study picture on cisoai.au.

```sh
python examples/cisoai_case_study.py out/case.svg
python -m isoscene.preview out/case.svg out/case.png --phone
python tests/test_examples.py
```

`SKILL.md` is the guide: workflow, coordinates, API, stacking and style. The repository doubles as
a Claude Code skill: link it into `~/.claude/skills/isoscene`.

```powershell
New-Item -ItemType Junction -Path "$HOME\.claude\skills\isoscene" -Target C:\code\isoscene
```

To use it from another project, either `pip install -e C:\code\isoscene` or put the folder on
`sys.path` in the scene script. Keep each scene script in the project that publishes the picture.

See `NOTICE.md` for the logos and icons.
