# SEHS4696-Development Environment

## Integrated Development Environment (IDE)

Install PyCharm using JetBrains Toolbox

## Python Interpreter

> 簡單講，Conda提供Python版本管理，Poetry提供Python virtual environment和packages管理

### Conda

```Bash
brew install anaconda
/opt/homebrew/anaconda3/bin/conda init zsh
# Restart terminal
```

### Poetry Environment

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

## Start with shared project

```Bash
git clone https://github.com/andrewfung729/SEHS4696-Tutorial.git
cd SEHS4696-Tutorial
poetry install
```

## References

- [https://docs.conda.io/projects/conda/en/latest/commands/index.html](https://docs.conda.io/projects/conda/en/latest/commands/index.html)
- [https://josix.tw/post/pipx-deep-dive/](https://josix.tw/post/pipx-deep-dive/)
- [https://blog.kyomind.tw/python-poetry/](https://josix.tw/post/pipx-deep-dive/)
- [https://python-poetry.org/docs/](https://josix.tw/post/pipx-deep-dive/)