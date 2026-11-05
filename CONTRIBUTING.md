# Contributing to Nirikshak

Thanks for your interest. Bug reports, documentation fixes, new attacks, new detectors and new
hardware runs are all welcome. By taking part you agree to follow the
[Code of Conduct](CODE_OF_CONDUCT.md).

## Before you start

- For a bug, open an [issue](https://github.com/dipankarchettri/nirikshak/issues) with the
  command you ran, what you expected and what happened.
- For anything larger than a small fix (a new attack, detector or change to the statistics),
  open an issue first so we can agree on the approach.
- Security problems: do not open a public issue; see [SECURITY.md](SECURITY.md).

## Development setup

```bash
git clone https://github.com/<your-username>/nirikshak.git   # your fork
cd nirikshak
python3 -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
python -m pytest -q
```

Python 3.11 or newer. `requirements.txt` pins the direct dependencies; `requirements.lock` is the
full environment we tested (Linux, Python 3.12). On Linux, read the `libgomp` note in the README
if you use Jupyter.

For the web app (Node 20 or newer):

```bash
cd web
npm ci
npm run lint
npm run build
```

## Making a change

1. Create a branch from an up-to-date `main`: `git checkout -b feature/short-name`.
2. Keep the change focused. Add or update tests in `tests/` for any behaviour you change.
3. Run `python -m pytest -q` (and `npm run lint && npm run build` in `web/` if you touched it).
4. If your change affects results, run `python -m src.main` and commit the regenerated files in
   `results/` and `web/src/results/` together with the code, so the numbers in the README stay
   reproducible.
5. Open a pull request against `main` and fill in the template. CI runs the tests and the web
   build on every pull request.

### Commit messages

| Prefix | Meaning |
| :--- | :--- |
| `feat:` | New feature |
| `fix:` | Bug fix |
| `docs:` | Documentation only |
| `test:` | Adding or fixing tests |
| `refactor:` | Code restructure, no behaviour change |
| `chore:` | Build, config or dependency changes |

## Where things live

| To add | Look at |
| :--- | :--- |
| An attack | `nirikshak/attacks/` (`base.py` defines the interface; see `intercept_resend.py`) |
| A detector | `nirikshak/detectors/`, then register it in `scripts/stress_test.py` |
| A noise or drift model | `nirikshak/noise/` |
| A test condition | `nirikshak/conditions.py` |
| Hardware batch logic | `nirikshak/hardware/` and `scripts/collect.py` |

## Results and claims

Nirikshak's value is that every number can be traced and reproduced. Please keep it that way:

- State the backend (or simulator setting) with every number, and give intervals where the
  scorecard does.
- Do not claim detection results from runs with mismatched timing between honest and attacked
  circuits (see "What real hardware taught us" in the README).
- Label simulated attacks as simulated.

## Sharing IBM hardware runs

Hardware data from more machines and dates is one of the most useful contributions.

- Plan with `python scripts/collect.py --batch <n>` first (free) and test on the simulator.
- Commit the block dataset that `collect.py --fetch` writes to `data/hardware/<job_id>.parquet`,
  and give the job ID, backend and date in the pull request. The job metadata and calibration
  snapshots go to `data/raw/<job_id>.json`, which is git-ignored; attach that file to the pull
  request so the run can be checked.
- Never commit `.env`, `qiskit-ibm.json` or any API key. Both are git-ignored; check
  `git status` before committing.

## Licence

By contributing, you agree that your contributions are licensed under the [MIT License](LICENSE).
