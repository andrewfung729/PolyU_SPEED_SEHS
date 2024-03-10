# Development Environment Setup

用Mac的同學有福了，唔使再痛苦咁搞Tomcat、OpenJDK。用 [Homebrew](Homebrew.md) 啦! \
用Docker的同學有福了，唔使再痛苦咁搞MariaDB、MySQL Workbench。裝 [Docker](Docker.md) 啦!

## Integrated Development Environment (IDE)

For developing J2EE applications, I recommend using the IntelliJ IDEA Ultimate Edition. It offers comprehensive support
for Java EE, Spring, and other enterprise technologies.

1. Install JetBrains Toolbox using Homebrew
    ```bash
    brew install jetbrains-toolbox
    ```

2. Install IntelliJ IDEA Ultimate Edition using JetBrains Toolbox
   <img alt="Jetbrains Toolbox" src="jetbrains-toolbox.png" width="400"/>

## Java Development Kit (JDK)

- Install the latest OpenJDK using Homebrew
   ```bash
   brew install openjdk
   ```
- For the system Java wrappers to find this JDK, symlink it with
  ```bash
  sudo ln -sfn /opt/homebrew/opt/openjdk/libexec/openjdk.jdk /Library/Java/JavaVirtualMachines/openjdk.jdk
  ```

- If you need to have openjdk first in your PATH, run (Optional)
    ```bash
    echo 'export PATH="/opt/homebrew/opt/openjdk/bin:$PATH"' >> ~/.zshrc
    ```

- For compilers to find openjdk you may need to set (Optional)
    ```bash
    export CPPFLAGS="-I/opt/homebrew/opt/openjdk/include"
    ```
- The JDK path you need to add to IntelliJ IDEA is
    ```bash
    /Library/Java/JavaVirtualMachines/openjdk.jdk/Contents/Home
    ```

## Java Servlet Container

Install Apache Tomcat using Homebrew

```bash
brew install tomcat
```

## Database Management System

Install MariaDB & PhpMyAdmin using Andrew Fung's Docker
Templates: [Tomcat-MariaDB-phpMyAdmin All-in-One Docker Template](https://github.com/andrewfung729/tomcat-mariadb-phpmyadmin-aio-docker) \
Don't forget to follow the instructions in the README file!