# macOS Installation Guide

Follow these steps to install the necessary tools for the **Orchestration Fundamentals for Agentic Development** course on macOS.

## 1. Install Homebrew

If you do not have Homebrew installed, open your Terminal and run:

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

## 2. Install Git

Use Homebrew to install Git:

```bash
brew install git
```

Verify the installation:

```bash
git --version
```

## 3. Install Python 3

Use Homebrew to install Python 3:

```bash
brew install python
```

Verify the installation:

```bash
python3 --version
```

## 4. Install Node.js (Prerequisite for Claude Code)

Claude Code requires Node.js (version 18 or later).

```bash
brew install node
```

Verify the installation:

```bash
node -v
npm -v
```

## 5. Install Claude Code

Install Claude Code globally using `npm`:

```bash
npm install -g @anthropic-ai/claude-code
```

Verify the installation by checking the version:

```bash
claude --version
```

Once installed, you may need to authenticate by running:

```bash
claude login
```

## 6. Install Visual Studio Code

Use Homebrew to install Visual Studio Code:

```bash
brew install --cask visual-studio-code
```

Verify the installation:

```bash
code --version
```

If the `code` command is not found, open VS Code, press `Cmd+Shift+P`, run **Shell Command: Install 'code' command in PATH**, then reopen your terminal.

## 7. Install VS Code Extensions

Install the following extensions, which are used during the breakout labs:

- **Colab in VS Code** ([googlecolab/colab-vscode](https://github.com/googlecolab/colab-vscode)) — connects a VS Code window to a Google Colab runtime
- **Code Runner** ([formulahendry/vscode-code-runner](https://github.com/formulahendry/vscode-code-runner)) — runs code snippets in many languages directly from the editor

Install from the command line:

```bash
code --install-extension google.colab
code --install-extension formulahendry.code-runner
```

Or install them from the Extensions view (`Cmd+Shift+X`) by searching for "Colab in VS Code" and "Code Runner".
