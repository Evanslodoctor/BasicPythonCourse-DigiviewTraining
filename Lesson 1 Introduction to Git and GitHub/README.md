### Generate SSH Key:

If you haven't already, generate an SSH key pair on your local machine. You can do this by running the following command in your terminal:

```bash

ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
```

Replace "your_email@example.com" with your actual email address.
x

### Add SSH Key to SSH Agent: Start the SSH agent and add your SSH private key to it:

```bash

eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_rsa
```

Make sure to replace ~/.ssh/id_rsa with the path to your private key if it's located elsewhere.

### Add SSH Key to GitHub:

Copy the SSH public key to your clipboard using the following command:

```bash

pbcopy < ~/.ssh/id_rsa.pub
```

If you're not on macOS, you might not have pbcopy. You can use cat ~/.ssh/id_rsa.pub and then copy the output manually.

Then, go to your GitHub account settings, navigate to SSH and GPG keys, and add a new SSH key. Paste your public key into the provided field.

### Test SSH Connection:

To ensure that everything is set up correctly, test your SSH connection to GitHub:

```bash

ssh -T git@github.com
```

You should see a message indicating successful authentication.

### Configure Git to Use SSH:

Configure Git to use SSH for GitHub repositories. If you have repositories already cloned via HTTPS, you can switch the remote URL to SSH. Inside the repository directory, run:

```bash

git remote set-url origin git@github.com:username/repository.git
```

Replace username with your GitHub username and repository with the name of your repository.

# Configuring Email and Username in Git

To associate your email and username with your Git commits, follow these steps:

## 1. Set Up Email

Open your terminal and run the following command:

```bash
git config --global user.email "your_email@example.com"

```

# Setting Up Username in Git

To associate your username with your Git commits, follow these steps:

## 1. Set Up Username

Open your terminal and run the following command:

```bash
git config --global user.name "Your Name"
```

# Verification of Git Configuration

After configuring your email and username in Git, you may want to verify that the settings are correctly applied. Here's how:

## 1. Verify Email Configuration

To check the email address associated with your Git commits, run the following command in your terminal:

```bash
git config --global user.email
```

# Verifying Username Configuration in Git

To ensure that your username is correctly configured in Git, follow these steps:

## 1. Verify Username Configuration

Open your terminal and run the following command:

```bash
git config --global user.name
```

# Setting Up Git Credential Helper

When working with Git over HTTPS, you can set up a credential helper to securely store your credentials. This allows Git to remember your username and password, so you don't have to enter them every time.

## 1. Check Git Version

Ensure you have Git version 1.7.10 or newer, as Git Credential Manager is included starting from this version.

## 2. Configure Git Credential Helper

Open your terminal and run the following command:

```bash
git config --global credential.helper store
```

# Push Changes to GitHub Repository Using GitHub CLI

If you have GitHub CLI (gh) installed, you can easily push changes to your GitHub repository from the command line.

## 1. Authenticate with GitHub

Before pushing changes, ensure you are authenticated with GitHub CLI by running the following command and following the prompts:

```sh
gh auth login
```

# Add changes to the staging area

```bash
git add .
```

# Commit changes with a commit message

```bash
git commit -m "Your commit message"
```

# Push changes to the remote repository

```bash
gh repo view owner/repo

```
