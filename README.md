# Spark with Python 3.12

## System Setup

```bash
# install pyenv if not installed
which pyenv || curl https://pyenv.run | bash

# install poetry with system's python interpreter, if not installed
which poetry || curl -sSL https://install.python-poetry.org | /usr/bin/python
```

## Project Setup

```bash
pyenv update
pyenv install 3.12.1
pyenv local 3.12.1

# tell poetry to use v3.12
poetry env use $(pyenv which python)
poetry install

# run the demo script
poetry run python spark-test.py
```
