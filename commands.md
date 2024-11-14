# Git Commands

## Update Packages
- `sudo apt-get update`

## Directory Operations
- **Create Directory**: `mkdir <directory_name>`
- **Navigate to Directory**: `cd <directory_name>`

## Initialize Git Repository
- `git init`

## Check Git Installation
- **Check Git Path**: `which git`

## File Operations
- **Create File**: `touch <file_name>`
- **Rename File**: `mv <old_name> <new_name>`

## View Directory Contents
- `ls`

## Git Status
- **Check Status**: `git status`

## Adding Files to Staging Area
- **Add Specific File**: `git add <file_name>`
- **Add All Files**: `git add .`

## Committing Changes
- **Commit with Message**: `git commit -m "your message"`

## Configuring Git
- **Set Global Username**: `git config --global user.name "<username>"`
- **Set Global Email**: `git config --global user.email "<email>"`

## Removing Files from Staging Area
- **Unstage File**: `git rm --cached <file_name>`

## Restore Changes
- **Restore File**: `git restore <file_name>`

## Viewing Commit Logs
- **Full Log**: `git log`
- **Compact Log**: `git log --oneline`

## Branch Operations
- **List Branches**: `git branch`
- **Create and Switch to New Branch**: `git checkout -b <branch_name>`
- **Switch Branches**: `git checkout <branch_name>`

## Viewing Command History
- `history`
