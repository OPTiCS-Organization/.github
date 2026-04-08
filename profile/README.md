# Introduction
> OPTiCS is help you to make your PC into cloud server without any extra rental cost.
> just execute single script in any PC.
> then you can deploy any project from home, at work, even on vacation!
> also you can use your Agent as a normal PC!

# Requirements
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

# Getting Started
To get started, you have to execute cURL Installation script below from the PC which is you want to change into Server.
then, follow script's instructions

## Installation of Agent Client
### Windows (PowerShell)
```Shell
curl.exe -fsSL https://github.com/OPTiCS-Organization/OPTiCS-Infra/raw/main/windows/install-agent.ps1 -o $HOME\install-agent.ps1; if ($?) { powershell -ExecutionPolicy Bypass -File $HOME\install-agent.ps1 }
```
### Arch Linux
```Shell
curl -fsSL https://github.com/OPTiCS-Organization/OPTiCS-Infra/raw/main/linux/install-agent.sh -o install-agent.sh && sh install-agent.sh
```

if installation successfully finished, you can access dashboard via http://localhost:5240/
> Note: Dashboard is only accessible when you access from local. any access from external service(and etc) will ignored from Agent Client due to Security.

## Sign In
You must have existing and verificated Hub account.
You can just sign up or sign in from [here](https://consoleoptics.vercel.app).

## Register Agent
You can register new Agent from Workspaces/Agent page.
Enter Agent Dashboard, Check displaying connection code from landing page.
Enter connection code from Hub Console, Workspaces/Agent page.
If connection code is valid and not expired, connection request will sent to Agent. You can check request from Agent Dashboard.
Click Accept Request.
Now it's done!

## Deploy Service
> Note: Currently OPTiCS doesn't support any framework. so you will need to write dockerfile/compose in your repository.
Move to Hub Console, Workspaces/Service page.
Click Deploy New Service Button.
Enter Service Information.
Hit Deploy Button.

You can check log via click service.
