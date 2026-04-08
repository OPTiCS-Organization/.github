## Introduction
> OPTiCS is help you to make your PC into cloud server without any extra rental cost.
> just execute single script in any PC.
> then you can deploy any project from home, at work, even on vacation!
> also you can use your Agent as a normal PC!

## Requirements
1. **Operating System**
> We are supporting few OS yet. we are planning to support another distro linux's.
> Check list below to view current supported OS.
  - Windows 10/11
  - Arch Linux 6.19.x

2. **Specs**
  - At Least 1GB RAM
  - At Least 1Core PC
  - At Least 5GB Storage
  - Internet Connection

## Getting Started
To get started, you have to execute command below to install Agent client

### Windows (PowerShell)
```Shell
curl.exe -fsSL https://github.com/OPTiCS-Organization/OPTiCS-Infra/raw/main/windows/install-agent.ps1 -o $HOME\install-agent.ps1; if ($?) { powershell -ExecutionPolicy Bypass -File $HOME\install-agent.ps1 }
```
### Arch Linux
```Shell
curl -fsSL https://github.com/OPTiCS-Organization/OPTiCS-Infra/raw/main/linux/install-agent.sh -o install-agent.sh && sh install-agent.sh
```
