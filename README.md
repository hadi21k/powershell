# Setup Powershell prompt

### Install Nerd Fonts [Hack](https://github.com/ryanoasis/nerd-fonts/releases/tag/v2.1.0)

## Install Scoop:

```bash
iwr -useb get.scoop.sh | iex
```

```bash
scoop install curl sudi jq
```
## Install Git:

```bash
winget install -e --id Git.Git
```

## Install Neovim and Gcc:

```bash
scoop install neovim gcc
```

```bash
mkdir ./config/powershell
```

```bash
nvim user_profile.ps1
```

```bash
nvim $PROFILE.CurrentUserCurrentHost
```

## Add in $PROFILE.CurrentUserCurrentHost:

```bash
. $env:USERPROFILE\.config\powershell\user_profile.ps1
```

## Install oh-my-posh:

```bash
Install-Module posh-git -Scope CurrentUser -Force
```

```bash
Install-Module oh-my-posh -Scope CurrentUser -Force
```

### [Themes Link](https://ohmyposh.dev/docs/themes)

```bash
vim theme.omp.json
```

```bash
Add theme code
```

## Install Terminal Icons:

```bash
Install-Module -Name Terminal-Icons -Repository PSGallery -ForceImport-Module  Terminal-Icons
```

## Install PSReadLine - Autocompletion:

```bash
Install-Module -Name PSReadLine -AllowPrerelease -Scope CurrentUser -Force -SkipPublisherCheck
```

If it doesn't works delete -AllowPrerelease

## Set Prediction:

```bash
Set-PSReadLineOption -PredictionSource History
```

```bash
Set-PSReadLineOption -PredictionViewStyle ListView
```

