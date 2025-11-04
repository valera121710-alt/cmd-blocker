# CMD Blocker - Virus Protection Tool

🛡️ A security application that blocks Command Prompt and PowerShell to protect against malware and viruses.

## Features
- ✅ Blocks cmd.exe, powershell.exe, pwsh.exe
- ✅ GUI interface for easy control
- ✅ Auto-start with Windows
- ✅ Real-time protection
- ✅ Logging of blocked processes
- ✅ MSI installer for easy deployment

## Download
[📦 Download Installer](installer/CmdBlockerGUI-1.0.0.msi)

## How to Use
1. Download and run the MSI installer
2. Launch "CMD Blocker" from Start Menu
3. Click "Start Protection" to enable blocking
4. Application runs automatically on Windows startup

## System Requirements
- Windows 10/11
- Administrator rights for full protection
- Java Runtime (included in installer)

## Building from Source
```bash
# Compile
javac -d build/classes src/SimpleCmdBlocker.java

# Create JAR
jar cfe CmdBlocker.jar SimpleCmdBlocker -C build/classes .

# Create MSI installer
jpackage --name "CmdBlocker" --type msi --input . --main-jar CmdBlocker.jar --main-class SimpleCmdBlocker --win-shortcut --win-menu
