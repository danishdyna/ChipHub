# Install Docker - Windows
## Download & Compare Checksum
Docker Desktop for Windows - PowerShell  
https://docs.docker.com/desktop/install/windows-install/
```
cd %USERPROFILE%\Downloads
wget "https://desktop.docker.com/win/main/amd64/157355/Docker%20Desktop%20Installer.exe" -O DockerDesktop.exe
wget "https://desktop.docker.com/win/main/amd64/157355/checksums.txt" -O DockerDesktop.sum
(Get-FileHash .\DockerDesktop.exe).Hash
(Get-Content .\DockerDesktop.sum).Split()[0]
Write-Host -NoNewline "Compare sumcheck: "; (Get-FileHash .\DockerDesktop.exe).Hash -eq (Get-Content .\DockerDesktop.sum).Split()[0]
```
## Install
```
DockerDesktop.exe
```
