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
- git remote add origin git@github.com:Safiakhatoon767/birthday.git
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

### **git revert**

- **Create a New Directory**  
  ```bash
  mkdir merigithub
  cd merigithub/
  mkdir git_prac
  cd git_prac/
  git init
  ```

- **Create and Check Branches**  
  ```bash
  git branch          # List all branches
  git checkout -b dev # Create and switch to a new branch "dev"
  git checkout -b stagining # Create and switch to "stagining" branch
  git branch          # Verify all branches
  ```

- **Make Changes and Commit**  
  ```bash
  touch master1.txt
  git add master1.txt
  git commit -m "add this in master"
  ```

- **Working on Features**  
  ```bash
  vim feature-1.txt
  git add feature-1.txt
  git commit -m "add this file in dev"

  vim feature-2.txt
  git add feature-2.txt
  git commit -m "add this file in dev"

  vim feature-3.txt
  git add feature-3.txt
  git commit -m "add this file in dev"
  ```

- **View Commit Logs**  
  ```bash
  git log --oneline
  ```

- **Revert a Commit**  
  ```bash
  git revert <commit-hash>
  ``` 

### **Rebase Workflow Commands**

#### **Rebasing Between Branches**

- **Switch to the Development Branch**  
  ```bash
  git checkout dev
  ```

- **Add and Commit Changes in `dev` Branch**  
  ```bash
  vim file8.txt
  git add file8.txt
  git commit -m "add file8.txt"

  vim file6.txt
  git add file6.txt
  git commit -m "add file6.txt"
  ```

- **View Commit History**  
  ```bash
  git log --oneline
  ```

- **Switch Back to the Master Branch**  
  ```bash
  git checkout master
  ```

- **Add and Commit Changes in `master` Branch**  
  ```bash
  vim file3.txt
  git add file3.txt
  git commit -m "add file3.txt"
  ```

- **Rebase `dev` Branch into `master`**  
  ```bash
  git rebase dev
  ```

- **Check Commit History After Rebase**  
  ```bash
  git log --oneline
  ```
  ### **Cherry-Pick Commands and Explanation**

#### **Steps Performed:**

1. **Create New Files in `dev` Branch:**
   - Created `imp.txt` and committed with the message: `important file`.
   - Created `notomp.txt` and committed with the message: `not imp`.

2. **Switch to `master` Branch:**
   - Used `git checkout master` to move from `dev` to `master`.

3. **Cherry-Pick Commit from `dev` to `master`:**
   - Command: `git cherry-pick eedac82`
     - This picks the commit `eedac82` (e.g., the commit for `important file`) from `dev` and applies it to `master`.

#### **Resulting Commit Log in `master` After Cherry-Pick:**

1. The `eedac82` commit (important file) is now part of `master`.
2. Commits from `dev` not cherry-picked (e.g., `not imp`) remain in `dev` only.


### **Stashing Commands and Explanation**

#### **Steps Performed:**

1. **Check Status of Changes:**
   - `git status` to view modified files (`feature-3.txt` was modified).

2. **Stash Changes Temporarily:**
   - Command: `git stash`
     - Temporarily saves changes in `feature-3.txt` without committing.

3. **Modify and Commit Another File:**
   - Edited and committed `feature-1.txt` with the message: `comple my work`.

4. **Show Stash Details:**
   - Command: `git stash show`
     - Displays the files saved in the most recent stash.

5. **Apply Stash and Remove it from Stash List:**
   - Command: `git stash pop`
     - Restores the stashed changes and removes the stash entry.

6. **Complete Work on Restored File:**
   - Edited `feature-3.txt` again.
   - Staged and committed it with the message: `stash file work done`.

#### **Result:**
- Changes in `feature-3.txt` were stashed, restored, and committed after completing other work.

  ### Command List: Squash Merge and Related Actions

- **List all branches**:  
  ```bash
  git branch
  ```

- **Rebase master from origin**:  
  ```bash
  git pull origin master --rebase
  ```

- **View commit history (short format)**:  
  ```bash
  git log --oneline
  ```

- **Switch to `dev` branch**:  
  ```bash
  git checkout dev
  ```

- **Switch to `master` branch**:  
  ```bash
  git checkout master
  ```

- **Perform a squash merge from `dev` branch**:  
  ```bash
  git merge --squash dev
  ```

- **Check status after squash merge**:  
  ```bash
  git status
  ```

- **Stage a file (`notomp.txt`)**:  
  ```bash
  git add notomp.txt
  ```

- **Commit the squash merge**:  
  ```bash
  git commit -m "Squash merge from dev branch"
  ```
### Commands for Resolving Merge Conflicts

- **List all branches**:  
  ```bash
  git branch
  ```

- **Modify file (`feature-1.txt`)**:  
  ```bash
  vim feature-1.txt
  ```

- **Stage changes**:  
  ```bash
  git add feature-1.txt
  ```

- **Commit the staged changes**:  
  ```bash
  git commit -m "add feature1 changes"
  ```

- **Switch to `dev` branch**:  
  ```bash
  git checkout dev
  ```

- **Make changes in `dev` branch (`feature-1.txt`)**:  
  ```bash
  vim feature-1.txt
  git add feature-1.txt
  git commit -m "this is my dev feature1 changes"
  ```

- **Switch back to `master` branch**:  
  ```bash
  git checkout master
  ```

- **Merge `dev` branch into `master`**:  
  ```bash
  git merge dev
  ```

- **Resolve merge conflict in `feature-1.txt`**:  
  Edit the file (`vim feature-1.txt`) to fix conflicts manually.

- **Check file status**:  
  ```bash
  git status
  ```

- **Stage the resolved file**:  
  ```bash
  git add feature-1.txt
  ```

- **Commit the resolved changes**:  
  ```bash
  git commit -m "solve merge conflict error"
  ```
  

