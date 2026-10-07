# Viewer Test — CI/CD Monitoring Test App

Minimal Python test application for CI/CD monitoring.

## Structure

```text
.
├── app/
│   └── calculator.py
├── tests/
│   └── test_calculator.py
├── .github/
│   └── workflows/
│       └── ci.yml
├── requirements.txt
└── README.md
```

## Setup

```bash
pip install -r requirements.txt
```

## Run tests

```bash
pytest -v
```

## CI

GitHub Actions workflow (`.github/workflows/ci.yml`) runs on push/PR to `main`:
1. Checks out code
2. Sets up Python 3.10 / 3.11 / 3.12
3. Installs dependencies
4. Runs `pytest -v`
