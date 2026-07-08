# 225-starter-files
Hello world!
A collection of files and folders containing the starter project for use in Champlain College WEBD-225 web course. 

# Cloning a Remote Repository in VS Code

This document covers the process of cloning an existing remote repository (for example, one hosted on GitHub) and creating a local copy of it on your machine using VS Code's built-in tools.

## Before You Start

You will need:

- VS Code installed
- Git installed on your machine
- The URL of the remote repository you want to clone

To confirm Git is installed, open a terminal (any terminal, not just VS Code's) and run:

```
git --version
```

If you see a version number, you are ready to proceed.

## Step 1: Copy the Repository URL

Go to the remote repository's page (GitHub, GitLab, or similar). Find the "Code" button and copy the URL. It will look something like:

```
https://github.com/username/repo-name.git
```

## Step 2: Open the Command Palette in VS Code

Open VS Code. Open the Command Palette using one of the following:

- Windows/Linux: Ctrl + Shift + P
- Mac: Cmd + Shift + P

## Step 3: Run the Clone Command

Type the following into the Command Palette:

```
Git: Clone
```

Select it when it appears in the list.

VS Code will then prompt you to paste the repository URL. Paste the URL you copied in Step 1 and press Enter.

## Step 4: Choose a Local Folder

VS Code will ask where to save the cloned repository on your machine. Choose a parent folder. VS Code will create a new folder inside it, named after the repository, and this new folder becomes your local root.

For example, if you choose to save inside `Documents/Projects`, and the repository is named `repo-name`, your local root will be:

```
Documents/Projects/repo-name
```

## Step 5: Open the Cloned Repository

After cloning finishes, VS Code will show a notification asking if you want to open the cloned repository. Click "Open."

If you miss the notification, you can open it manually:

- File → Open Folder...
- Navigate to the folder created in Step 4
- Select it

## Step 6: Confirm the Clone

Open the terminal in VS Code (View → Terminal, or Ctrl + `) and run:

```
git status
```

You should see output similar to:

```
On branch main
Your branch is up to date with 'origin/main'.
nothing to commit, working tree clean
```

This confirms two things: your local root is correctly linked to the remote, and your files match what is on the remote.

## Summary

| Step | Action |
|------|--------|
| 1 | Copy the remote repository URL |
| 2 | Open the Command Palette |
| 3 | Run "Git: Clone" and paste the URL |
| 4 | Choose where to save the local folder |
| 5 | Open the cloned folder in VS Code |
| 6 | Run `git status` to confirm the link |

Once these steps are complete, your local root is a full working copy of the remote repository, tracked by Git, and ready for editing.
