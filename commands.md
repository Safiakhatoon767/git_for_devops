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

## Directory Operations
- **Create Directory**: `mkdir github`
- **Change Directory**: `cd github/`

## Cloning Repositories
- **Clone Repository**: `git clone https://github.com/Safiakhatoon767/git_for_devops.git`

## File Editing and Staging
- **Edit File**: `vim README.md`
- **Add File to Staging Area**: `git add README.md`

## Committing Changes
- **Commit Changes with Message**: `git commit -m "your message"`

## Remote Repository Management
- **Set Remote URL**: `git remote set-url origin origin https://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@github.com/Safiakhatoon767/git_for_devops.git
- **View Remote URLs**: `git remote -v`
- **Remove Remote**: `git remote remove origin`
- **Add New Remote**: `git remote add origin <repository_url>`

## Pushing Changes
- **Push Changes to Remote**: `git push`
- **Push with Upstream**: `git push --set-upstream origin main`
- **Force Push with Upstream**: `sudo git push --set-upstream origin main`

## Pulling and Rebasing
- **Pull with Rebase**: `git pull origin main --rebase`
- **Continue Rebase**: `git rebase --continue`

## Checking Status
- **Check Git Status**: `git status`

## View and Edit File Contents
- **View File Content**: `cat README.md`


## Directory Navigation
- **Navigate to .ssh Directory**: `cd .ssh`
- **Go Back to Previous Directory**: `cd ..`
- **Print Working Directory Path**: `pwd`

## SSH Key Management
- **Generate SSH Key**: `ssh-keygen`
- **View SSH Public Key**: `cat id_ed25519.pub`

## File Management
- **Create or Edit File**: `vim safia.txt`

## Staging and Committing Changes
- **Add File to Staging**: `git add safia.txt`
- **Commit with Message**: `git commit -m "add karo meri file haha"`

## Remote Repository Management
- **View Remote URLs**: `git remote -v`
- **Set Remote URL to SSH**: `git remote set-url origin git@github.com:Safiakhatoon767/git_for_devops.git`

## Checking Status
- **Check Git Status**: `git status`

  

# Git Commands - Branching Strategies

## Basic Commands
- **Clear Terminal Screen**: `clear`
- **List Files and Directories**: `ls`

## Directory Navigation
- **Navigate to a Directory**: `cd github/`
- **Navigate to Project Directory**: `cd git_for_devops/`

## Branch Management
- **List Branches**: `git branch`
- **Create and Switch to New Branch (staging)**: `git checkout -b staging`
- **Create and Switch to New Branch (dev)**: `git checkout -b dev`
- **Switch to Existing Branch**: `git checkout <branch_name>`

## File Management
- **Create or Edit File**: `vim branching.md`

## Staging and Committing Changes
- **Add File to Staging**: `git add branching.md`
- **Commit with Message**: `git commit -m "adding branching.md strategy by safia"`

## Merging Branches
- **Merge Branch into Current Branch**: `git merge <branch_name>`

## Pushing Changes
- **Push Branch to Remote Repository**: `git push origin staging`

## Viewing Logs and Status
- **View Compact Commit Log**: `git log --oneline`
- **Check Git Status**: `git status`


