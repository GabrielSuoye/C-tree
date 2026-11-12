# C-tree

A simple tree directory viewer written in C inspired by Hayyoth on YouTube.

## Features

- get path
- walk(path)
  - if is dir -> walk(sub dir)
  - if is file -> print(file)

- coming soon
  - depth control (-L)
  - directory only toggle (-d)
  - hidden file and dotfile filtering
  - infinite loop protection against symlinks (symbolic link back to parent directory)
  - return size of directory alongside the directory name

## Prerequsites

Must have a toolchain installed on your operating system.

Installation via the terminal:

- Linux
  - Ubuntu/Debian:

    ```bash
    sudo apt update && sudo apt install build-essential
    ```

  - Fedora/CentOS/RHEL:

    ```bash
    sudo dnf groupinstall "Development Tools"
    ```

- Windows
  - Install MinGW-w64 (via MSYS2) to get GCC.

## Clone the repository

```bash
git clone https://github.com/GabrielSuoye/c-tree
```

## Build the application

```bash
cd src
```

```bash
gcc tree.c -o tree
```
