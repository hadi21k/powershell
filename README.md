install nerd fonts
Install scoop commands:
--- iwr -useb get.scoop.sh | iex
--- scoop install curl sudi jq
Install Git:
--- winget install -e --id Git.Git
Install Neovim and Gcc:
--- scoop install neovim gcc
--- mkdir ./config/powershell
--- nvim user_profile.ps1
--- nvim $PROFILE.CurrentUserCurrentHost
. $env:USERPROFILE\.config\powershell\user_profile.ps1
--- Install-Module posh-git -Scope CurrentUser -Force
--- Install-Module oh-my-posh -Scope CurrentUser -Force
Install Terminal Icons:
--- Install-Module -Name Terminal-Icons -Repository PSGallery -ForceImport-Module  Terminal-Icons
Install PSReadLine - Autocompletion
--- Install-Module -Name PSReadLine -AllowPrerelease -Scope CurrentUser -Force -SkipPublisherCheck ( it may not work delete -AllowPrerelease ) 
--- Set-PSReadLineOption -PredictionSource History
--- Set-PSReadLineOption -PredictionViewStyle ListView

