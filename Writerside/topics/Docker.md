# Docker Installation

## Mac

@use [Mac: Homebrew](Homebrew.md)

Recommended Docker management tools:

| Recommendation | Tools                         |
|----------------|-------------------------------|
| Highest        | Orbstack                      |
| Medium         | Docker CLI with VSCode Plugin |
| Least          | Docker Desktop                |

### Install Orbstack

Use Homebrew to install Orbstack:

```bash
brew install orbstack
```

### Install Docker CLI

1. Use Homebrew to install Docker CLI
    ```bash
    brew install --formula docker
    ```

2. Search docker in VSCode Extensions and install the Docker extension
   @see [Docker in Visual Studio Code](https://code.visualstudio.com/docs/containers/overview)

### Install Docker Desktop

Use Homebrew to install Docker Desktop

```bash
brew install --cask docker
```

### Uninstall Docker or Docker Desktop

Use Homebrew to install Docker Desktop

```Bash
brew uninstall --cask docker --force
brew uninstall --formula docker --force
```

## Linux

Install Docker using the official script

```bash
curl -fsSL https://get.docker.com -o get-docker.sh
sh get-docker.sh
```

Then, add your user to the `docker` group

```bash
sudo usermod -aG docker $USER
```

## Windows

As I do not develop on Windows, I am unable to provide a specific setup guide for this platform. Contributions are
welcome; if you wish to add a Windows guide, please submit a pull request. \
如果堅持要用Windows平台，可以試試WSL2 + Docker + VSCode，詳情自研

- [https://docs.docker.com/desktop/wsl/](https://docs.docker.com/desktop/wsl/)
- [https://hackmd.io/@CynthiaChuang/Install-Docker-in-WSL2](https://hackmd.io/@CynthiaChuang/Install-Docker-in-WSL2)

## References

- https://docs.docker.com
- https://github.com/twtrubiks/docker-tutorial
