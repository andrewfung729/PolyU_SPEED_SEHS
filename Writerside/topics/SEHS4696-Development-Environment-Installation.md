# SEHS4696 Development Environment

## Integrated Development Environment (IDE)

Install PyCharm using JetBrains Toolbox

## Python Interpreter

Recommended Python environment setup:
> ❗❗❗ 提供兩個較方便做法，請按照自己嘅需要選擇一個

1. Pyenv + Poetry
2. Conda + Poetry

## Poetry

Use Pipx to install Poetry

```Bash
brew install pipx

# Ensure pipx path, please reopne terminal after running this command
pipx ensurepath

# Install Poetry
pipx install poetry

# Enable virtualenvs in project
poetry config virtualenvs.in-project true
```

## Pyenv + Poetry

> Pyenv提供Python versions管理，Poetry提供Python virtual environment和packages管理

### Pyenv

Install Pyenv using Homebrew

```Bash
brew install pyenv
echo 'export PYENV_ROOT="$HOME/.pyenv"' >> ~/.zshrc
echo '[[ -d $PYENV_ROOT/bin ]] && export PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.zshrc
echo 'eval "$(pyenv init -)"' >> ~/.zshrc
# Restart terminal
```

Install latest Python 3.11 using Pyenv

```Bash
pyenv install 3.11 
pyenv global 3.11
```

## Conda + Poetry

> Conda提供Python versions同virtual environment管理，Poetry提供python packages管理

### Conda

Install Anaconda using Homebrew

```Bash
brew install anaconda
/opt/homebrew/anaconda3/bin/conda init zsh
# Restart terminal
```

Create a new Conda environment

```Bash
conda create -n sehs4696 python=3.11

# Activate the environment before installing packages
conda activate sehs4696
```

## Start with shared project

```Bash
git clone https://github.com/andrewfung729/SEHS4696-Tutorial.git
cd SEHS4696-Tutorial

# check your python interpreter path and version
which python
python --version

# use poetry to install dependencies
poetry install
```

## References

- [https://github.com/pyenv/pyenv](https://github.com/pyenv/pyenv)
- [https://docs.conda.io/projects/conda/en/latest/commands/index.html](https://docs.conda.io/projects/conda/en/latest/commands/index.html)
- [https://josix.tw/post/pipx-deep-dive/](https://josix.tw/post/pipx-deep-dive/)
- [https://blog.kyomind.tw/python-poetry/](https://josix.tw/post/pipx-deep-dive/)
- [https://python-poetry.org/docs/](https://josix.tw/post/pipx-deep-dive/)