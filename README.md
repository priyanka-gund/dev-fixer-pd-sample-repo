# sample-repo

Minimal repo for the dev-fixer-pd POC. `calc/calculator.py`'s `subtract()` has a
deliberate bug (`return a + b` instead of `a - b`), which makes
`tests/test_calculator.py::test_subtract` fail.

```
pip install -r requirements.txt
pytest -q
```

This repo is meant to be pushed to its own GitHub remote and mounted into a
Managed Agents session (see `RUNBOOK.md` Steps 4-5 in the parent project).

