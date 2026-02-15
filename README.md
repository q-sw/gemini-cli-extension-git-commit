# Gemini CLI Extension: git-commit

This Gemini CLI extension automates the creation of commit messages following the [Angular convention](https://github.com/angular/angular.js/blob/master/DEVELOPERS.md#-git-commit-guidelines).

## Features

- **Automatic Analysis**: Analyzes the `diff` of modified files to understand changes.
- **Angular Compliance**: Generates messages in the format `<type>(<scope>): <description>`.
- **Git Automation**: Automatically executes `git add` and `git commit` for you.
- **Smart Management**: Capable of splitting changes into multiple commits if necessary.

## Installation

### Local Installation

If you have cloned this repository, you can install the extension locally:

```bash
gemini extension install --local .
```

### Installation from GitHub

You can install the extension directly from the remote repository:

```bash
gemini extension install github:q-sw/git-commit
```

## Usage

Once installed, you can use the following command in any Git repository:

```bash
/git-commit
```

The assistant will analyze your uncommitted changes, suggest a message, and perform the commit if you validate (or automatically depending on its configuration).

## File Structure

- `gemini-extension.json`: Extension configuration file.
- `commands/git-commit.toml`: Command definition and agent prompt.
- `GEMINI.md`: (Optional) Specific context file for the extension.

---

[Version française (README.fr.md)](./README.fr.md)
