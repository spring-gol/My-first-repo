# My-first-repo
Just testing github
# ─────────────────────────────────────────────────────────────────────────────
# Project: simple-cli
# A minimal Python CLI project with unit tests and GitHub Actions CI.
# ─────────────────────────────────────────────────────────────────────────────


# ============================== .gitignore ===================================
# file: .gitignore
.venv/
__pycache__/
*.pyc
.coverage
dist/
*.egg-info/


# ============================ requirements.txt ===============================
# file: requirements.txt
click==8.1.7
pytest==8.2.1


# ============================== pyproject.toml ===============================
# file: pyproject.toml
[build-system]
requires = ["setuptools>=68", "wheel"]
build-backend = "setuptools.build_meta"

[project]
name = "simple-cli"
version = "0.1.0"
description = "A tiny Python CLI with tests and GitHub Actions CI."
readme = "README.md"
requires-python = ">=3.9"
dependencies = ["click>=8.1.7"]

[tool.pytest.ini_options]
addopts = "-q"


# ================================= README.md =================================
# file: README.md
# simple-cli
A tiny Python CLI to compute stats over numbers.

## Setup
```bash
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate
pip install -r requirements.txt
