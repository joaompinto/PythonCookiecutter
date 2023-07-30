# PythonCookiecutter

This repository provides a cookicutter recipe for a new package.

What is included:
- automatic versioning using [setuptools_scm](https://pypi.org/project/setuptools-scm/)
- pre-commit hooks:
    - black
    - end-of-file-fixer
    - mixed-line-ending
    - pytest and pytes-tcover
    - ruff
    - trailing-whitespace
- invoke tasks: setup, test, test-only, cover, cover-only
- github actions for automated pipy releases
- vscode settings
    - exclude build test and cache directories
    - setup "Run" action to run pytest

## How to use:
```sh
pip install cruft

cruft https://github.com/joaompinto/PythonCookiecutter.git

cd project_directory
git init
git add .
git commit -a -m "Initial commit"
pip install --user -r requirements-dev.txt
pre-commit install
tox
```
