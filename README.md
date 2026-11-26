# BREyeCandy

A BRBuild project for non-operational and visual-only vehicles that complement the BRTrains family.

## Build

From this directory:

```bash
uv venv --python 3.13 .venv
uv pip install --python .venv/bin/python pillow pyyaml nml
BRBUILD_DIR=/path/to/BRBuild .venv/bin/python build.py --log --docs
```

A successful build writes `docs/generated/manifest.json`, the BRDocs project manifest.

## Layout

- `BRBuild.yaml` — BRBuild project configuration and BRDocs opt-in
- `build.py` — project-local BRBuild launcher
- `src/grf/GRF.yaml` — GRF metadata
- `src/vehicles/` — eye-candy vehicle definitions and artwork
- `docs/generated/` — generated BRDocs manifest
