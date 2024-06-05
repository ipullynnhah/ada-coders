# Digital Course: Git

## TOC

- [Digital Course: Git](#digital-course-git)
  - [TOC](#toc)
  - [What's `git`?](#whats-git)
  - [Installation](#installation)
    - [MAC OS](#mac-os)
    - [Linux (Debian)](#linux-debian)
    - [Windows](#windows)
  - [Configuring Git](#configuring-git)
  - [Git Repository Types](#git-repository-types)
    - [Local Repository](#local-repository)
    - [Remote Repository](#remote-repository)
    - [Cloned Repository](#cloned-repository)
  - [Git Commands](#git-commands)
    - [git add](#git-add)
    - [git branch](#git-branch)
    - [git checkout](#git-checkout)
    - [git clone](#git-clone)
    - [git commit](#git-commit)
    - [git fetch](#git-fetch)
    - [git init](#git-init)
    - [git log](#git-log)
    - [git pull](#git-pull)
    - [git push](#git-push)
    - [git restore](#git-restore)
    - [git status](#git-status)

## What's `git`?

Git is a distributed version control system designed for speed and efficiency, created by Linus Torvalds in 2005. Here are some key aspects of Git:

- **Distributed Nature**: Every developer has a full copy of the repository, enhancing collaboration and redundancy.
- **Speed and Efficiency**: Git handles large projects with many branches and merges efficiently.
- **Branching and Merging**: Git allows quick creation, merging, and deletion of branches, facilitating experimental development and collaboration.
- **Commit History**: Maintains a detailed history of changes with unique SHA-1 hashes for each change.
- **Staging Area**: Uses a staging area to prepare commits, allowing selective staging of changes.
- **Collaboration Tools**: Integrates with platforms like GitHub, GitLab, and Bitbucket, offering pull requests, code reviews, and issue tracking.
- **Open Source**: Free and open-source with a large contributing community.
- **Reliability and Flexibility**: Known for robustness and flexibility, popular for a wide range of projects.

Git is an essential tool for modern software development, providing powerful version control and collaboration capabilities.

## Installation

### MAC OS

1. **Install Homebrew** (if not already installed):

   ```sh
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   ```

2. **Install Git**
   ```sh
   brew install git
   ```
3. **Verify Installation**:
   ```sh
   git --version
   ```

### Linux (Debian)

1. **Update package index**:
   ```sh
   sudo apt update
   ```
2. **Install Git**
   ```sh
   sudo apt install git
   ```
3. **Verify Installation**:
   ```sh
   git --version
   ```

### Windows

1. **Download**: Go to the [Git for Windows](https://gitforwindows.org/) website and download the latest installer.
2. **Run the Installer**: Follow the installation prompts. You can keep the default settings unless you have specific preferences.
3. **Verify Installation**:
   ```sh
   git --version
   ```

## Configuring Git

To set up your Git configuration, you need to specify your user name and email address. These will be associated with your commits.

1. **Set Your User Name**:
   ```sh
   git config --global user.name "NAME"
   ```
2. **Set Your Email**:
   ```sh
   git config --global user.email "EMAIL"
   ```

Make sure to replace `NAME` and `EMAIL` with your actual name and email address.

## Git Repository Types

Git repositories come in various types, each serving different purposes and workflows.

### Local Repository

- A local repository exists on your local machine.
- It contains the entire project history and allows you to work offline.
- You can create a local repository using the `git init` command.

### Remote Repository

- A remote repository is hosted on a remote server, such as GitHub, GitLab, or Bitbucket. - It serves as a centralized location for collaboration and backup.
- You can push your changes to a remote repository using the `git push` command and fetch changes from it using `git fetch` or `git pull`.

### Cloned Repository

- A cloned repository is a copy of another repository on your local machine.
- It includes all the commits, branches, and history of the original repository.
- You can clone a repository using the `git clone` command.

Understanding these different types of Git repositories helps you effectively manage your projects and collaborate with others.

## Git Commands

### git add

- **Usage**: Adds changes in the working directory to the staging area.
- **Example**:
  - `git add <file_name>`
  - `git add .` (to add all changes)

### git branch

- **Usage**: Lists, creates, renames, or deletes branches.
- **Example**:
  - `git branch` (list branches)
  - `git branch <branch_name>` (create a new branch)
  - `git branch -d <branch_name>` (delete a branch)

### git checkout

- **Usage**: Switches between branches or restores files from the repository.
- **Example**:
  - `git checkout <branch_name>` (switch to a branch)
  - `git checkout -b <new_branch_name>` (create and switch to a new branch)

### git clone

- **Usage**: Clones a repository from a remote server to your local machine.
- **Example**:
  - `git clone <repository_URL>`

### git commit

- **Usage**: Records changes in the staging area to the repository with a commit message.
- **Example**:
  - `git commit -m "Commit message"`

### git fetch

- **Usage**: Downloads objects and references from another repository.
- **Example**:
  - `git fetch`

### git init

- **Usage**: Initializes a new Git repository in the current directory.
- **Example**:
  - `git init`

### git log

- **Usage**: Displays the commit history.
- **Example**:
  - `git log`
  - `git log --oneline` (show commits in a single line)

### git pull

- **Usage**: Fetches changes from a remote repository and merges them into the current branch.
- **Example**:
  - `git pull origin <branch_name>`

### git push

- **Usage**: Uploads local repository changes to a remote repository.
- **Example**:
  - `git push`

### git restore

- **Usage**: Restores files in the working directory to their state at a specific commit.
- **Example**:
  - `git restore <file>` (reverts changes made to the specified file in your working directory)
  - `git restore --staged` (Unstages changes made to the specified file in the staging area)

### git status

- **Usage**: Displays the status of the working directory and staging area.
- **Example**:
  - `git status`

These Git commands are essential for version control and collaboration in software development projects.
