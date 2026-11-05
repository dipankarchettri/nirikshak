## What this changes

## Why

## Checks

- [ ] `python -m pytest -q` passes
- [ ] `npm run lint && npm run build` in `web/` passes (if the web app changed)
- [ ] If results changed: ran `python -m src.main` and committed `results/` and `web/src/results/`
- [ ] Every new number names its backend or simulator setting
- [ ] No API keys, `.env` or `qiskit-ibm.json` in the diff
