```Powershell
oh-my-posh init pwsh --config "$env:POSH_THEMES_PATH/emodipt-extend.omp.json" | Invoke-Expression

$env:VIRTUAL_ENV_DISABLE_PROMPT = 0
#34de4b3d-13a8-4540-b76d-b9e8d3851756 PowerToys CommandNotFound module

#Import-Module "C:/Program Files/PowerToys/WinUI3Apps/../WinGetCommandNotFound.psd1"
#34de4b3d-13a8-4540-b76d-b9e8d3851756

#34de4b3d-13a8-4540-b76d-b9e8d3851756 PowerToys CommandNotFound module
Import-Module "C:/Program Files/PowerToys/WinGetCommandNotFound.psd1"
#34de4b3d-13a8-4540-b76d-b9e8d3851756

function winget-install {
  param(
    [Parameter(Mandatory = $true)]
    [string] $packageName,

    [Parameter(Mandatory = $true)]
    [string] $directoryName
  )

  $installPath = "D:\Program Files\$directoryName"

  winget install $packageName --location $installPath
}
```
