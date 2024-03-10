# Development Environment Setup

用Mac的同學有福了，唔使再痛苦咁搞Tomcat、OpenJDK。用Homebrew啦，非常方便。@use [Mac: Homebrew](Mac-Homebrew.md) \
用Docker的同學有福了，唔使再痛苦咁搞MariaDB、MySQL Workbench。用Docker Compose啦，非常方便。@use [Docker](Docker.md)

## Integrated Development Environment (IDE)

For developing J2EE applications, I recommend using the IntelliJ IDEA Ultimate Edition. It offers comprehensive support
for Java EE, Spring, and other enterprise technologies.

Install JetBrains Toolbox using Homebrew and then install IntelliJ IDEA Ultimate Edition:

```bash
brew install jetbrains-toolbox
```

## Java Development Kit (JDK)

Install the latest OpenJDK using Homebrew:

```bash
brew install openjdk
```

## Java Servlet Container

Install Apache Tomcat using Homebrew:

```bash
brew install tomcat
```

## Database Management System

@use [Docker](Docker.md)
Install MariaDB & PhpMyAdmin using
templates: [Tomcat-MariaDB-phpMyAdmin All-in-One Docker Template](https://github.com/andrewfung729/tomcat-mariadb-phpmyadmin-aio-docker) \
Don't forget to follow the instructions in the README file!