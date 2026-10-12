# Windows Installation Guide

Follow these steps to install the necessary tools for the **Orchestration Fundamentals for Agentic Development** course on Windows.

## 1. Install Git

Download and install Git for Windows from the official website:
[https://gitforwindows.org/](https://gitforwindows.org/)

During installation, the default options are generally fine.

Verify the installation by opening Command Prompt or PowerShell and running:

```powershell
git --version
```

## 2. Install Python 3

Download the latest Python 3 installer for Windows from the official website:
[https://www.python.org/downloads/windows/](https://www.python.org/downloads/windows/)

**Important:** Check the box that says "Add Python to PATH" during the installation process.

Verify the installation:

```powershell
python --version
```

## 3. Install Node.js (Prerequisite for Claude Code)

Claude Code requires Node.js (version 18 or later).

Download the Windows Installer (.msi) from the official Node.js website:
[https://nodejs.org/en/download/](https://nodejs.org/en/download/)

Verify the installation:

```powershell
node -v
npm -v
```

## 4. Install Claude Code

Open PowerShell or Command Prompt as Administrator and install Claude Code globally using `npm`:

```powershell
npm install -g @anthropic-ai/claude-code
```

Verify the installation by checking the version:

```powershell
claude --version
```

Once installed, you may need to authenticate by running:

```powershell
claude login
```

## 5. Install Visual Studio Code

Download and install Visual Studio Code from the official website:
[https://code.visualstudio.com/download](https://code.visualstudio.com/download)

During installation, make sure to check **"Add to PATH"** so the `code` command is available from the terminal.

Verify the installation by opening a new Command Prompt or PowerShell window and running:

```powershell
code --version
```

## 6. Install VS Code Extensions

Install the following extensions, which are used during the breakout labs:

- **Colab in VS Code** ([googlecolab/colab-vscode](https://github.com/googlecolab/colab-vscode)) — connects a VS Code window to a Google Colab runtime
- **Code Runner** ([formulahendry/vscode-code-runner](https://github.com/formulahendry/vscode-code-runner)) — runs code snippets in many languages directly from the editor

Install from the command line:

```powershell
code --install-extension google.colab
code --install-extension formulahendry.code-runner
```

Or install them from the Extensions view (`Ctrl+Shift+X`) by searching for "Colab in VS Code" and "Code Runner".

## 7. Clone Dependent Repositories

The breakout labs use two additional repositories. Clone them into a working folder of your choice, for example `C:\code`:

```powershell
mkdir C:\code
cd C:\code
git clone https://github.com/kpassoubady/claude-helper.git
git clone https://github.com/kpassoubady/password-strength-checker.git
```

Verify both folders were created:

```powershell
dir claude-helper, password-strength-checker
```
