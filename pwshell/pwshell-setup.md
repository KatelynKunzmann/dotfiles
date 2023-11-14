# Powershell setup in Windows Terminal

1) Make Windows PowerShell default shell in Terminal

2) Use Ubuntu theme with 50% transparency
    - with 'Use acrylic material in tab row' on

3) Check 'Run this profile as Administrator'

4) Install desired Nerd Font from https://www.nerdfonts.com/font-downloads
    Extract and copy font files to C:\Windows\fonts\

5) Install Terminal Icons: https://github.com/devblackops/Terminal-Icons
   
    Install-Module -Name Terminal-Icons -Repository PSGallery
   
    Import-Module -Name Terminal-Icons
   
    
7) Install autocompletion: https://github.com/PowerShell/PSReadLine

    Install-Module -Name PowerShellGet -Force
   
    Exit
   
    Install-Module PSReadLine -AllowPrerelease -Force
   
    Import-Module PSReadLine


9) Install z directory jumper
    
    Install-Module -Name z -Force



Terminal Settings:
Use the following profile for settings.json file
            {
                "commandline": "%SystemRoot%\\System32\\WindowsPowerShell\\v1.0\\powershell.exe -NoExit -NoLogo -ExecutionPolicy ByPass -Command neofetch",
                "font": 
                {
                    "face": "GohuFont 14 Nerd Font Mono"
                },
                "guid": "{61c54bbd-c2c6-5271-96e7-009a87ff44bf}",
                "hidden": false,
                "name": "Windows PowerShell",
                "opacity": 53,
                "useAcryLic": true
            },
