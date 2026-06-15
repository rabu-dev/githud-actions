# githud-actions

![CI](https://github.com/rabu-dev/githud-actions/actions/workflows/ci.yml/badge.svg)

Aprendiendo GitHub Actions con Python.

## Qué incluye

- **Tests**: `pytest` ejecutado en matrix de Python 3.10 → 3.14
- **Linter**: `ruff` para análisis estático y formateo
- **Deploy**: auto-deploy a GitHub Pages en push a `master`

## Desarrollo local

```bash
# Instalar dependencias
pip install -r requirements.txt

# Correr tests
python -m pytest -v

# Correr linter
ruff check .
ruff format --check .
```

## Estructura

```
├── main.py              # Código principal
├── test_main.py         # Tests con pytest
├── requirements.txt     # Dependencias
├── public/
│   └── index.html       # Landing page (GitHub Pages)
└── .github/
    └── workflows/
        └── ci.yml       # Pipeline CI/CD
```
