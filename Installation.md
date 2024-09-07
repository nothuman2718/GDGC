# Guide to Install Git and Github CLI

# Git installation : 

## For Windows

Install [winget tool](https://docs.microsoft.com/en-us/windows/package-manager/winget) if you don't already have it, then type this command in command prompt or Powershell.


```sh
winget install --id Git.Git -e --source winget
```

or visit : [https://git-scm.com/download/win](https://git-scm.com/download/win)

## For Linux

If you have Linux, I believe you can figure it out yourself. [:)](https://git-scm.com/download/linux)

## For MacOS

Homebrew
Install homebrew if you don't already have it, then:

```sh
brew install git
```

MacPorts
Install MacPorts if you don't already have it, then:

```sh
sudo port install git
```

or visit [https://git-scm.com/download/win](https://git-scm.com/download/win)

# GitHub CLI Installation

### macOS

`gh` is available via [Homebrew][], [MacPorts][], [Conda][], [Spack][], [Webi][], and as a downloadable binary including Mac OS installer `.pkg` from the [releases page][].

#### Homebrew

| Install:          | Upgrade:          |
| ----------------- | ----------------- |
| `brew install gh` | `brew upgrade gh` |

#### MacPorts

| Install:               | Upgrade:                                       |
| ---------------------- | ---------------------------------------------- |
| `sudo port install gh` | `sudo port selfupdate && sudo port upgrade gh` |


### Linux & BSD

`gh` is available via:
- [our Debian and RPM repositories](./docs/install_linux.md);
- community-maintained repositories in various Linux distros;
- OS-agnostic package managers such as [Homebrew](#homebrew), [Conda](#conda), [Spack](#spack), [Webi](#webi); and
- our [releases page][] as precompiled binaries.

For more information, see [Linux & BSD installation](./docs/install_linux.md).

### Windows

`gh` is available via [WinGet][], [scoop][], [Chocolatey][], [Conda](#conda), [Webi](#webi), and as downloadable MSI.

#### WinGet

| Install:            | Upgrade:            |
| ------------------- | --------------------|
| `winget install --id GitHub.cli` | `winget upgrade --id GitHub.cli` |

> **Note**  
> The Windows installer modifies your PATH. When using Windows Terminal, you will need to **open a new window** for the changes to take effect. (Simply opening a new tab will _not_ be sufficient.)

#### scoop

| Install:           | Upgrade:           |
| ------------------ | ------------------ |
| `scoop install gh` | `scoop update gh`  |

#### Chocolatey

| Install:           | Upgrade:           |
| ------------------ | ------------------ |
| `choco install gh` | `choco upgrade gh` |

#### Signed MSI

MSI installers are available for download on the [releases page][].

### Codespaces

To add GitHub CLI to your codespace, add the following to your [devcontainer file](https://docs.github.com/en/codespaces/setting-up-your-project-for-codespaces/adding-features-to-a-devcontainer-file):

```json
"features": {
  "ghcr.io/devcontainers/features/github-cli:1": {}
}
```
