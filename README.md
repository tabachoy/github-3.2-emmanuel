# Github Lesson 3.2

## Github authentication
GitHub authentication is the process of verifying the identity of users and their access rights to GitHub services and resources
### Common authentication methods
Username and Password:
: Sign in to your GitHub account using your username and password.
: If you have Two-Factor Authentication (2FA) enabled, you'll need to enter a verification code sent to your mobile device or authentication app.
: Once authenticated, you can access your GitHub account and repositories.

Personal Access Tokens (PAT):
: Sign in to your GitHub account.
: Go to your account settings.
: In the "Developer settings," select "Personal access tokens."
: Click "Generate token" and follow the prompts to create a token.
: Use this token for authentication in place of your password when interacting with GitHub via Git, API, or other tools.

SSH Keys:
: Generate an SSH key pair on your local machine using ssh-keygen.
: Add the public key to your GitHub account. You can copy it from your local machine and paste it into your GitHub account settings under "SSH and GPG keys."
: Use the private key for authentication when interacting with GitHub via SSH.

OAuth Apps:
: Create an OAuth App in your GitHub account settings.
: Obtain client credentials (Client ID and Client Secret) for your OAuth App.
: Implement the OAuth flow in your application, which typically involves redirecting users to GitHub for authentication and obtaining an access token.
: Use the access token for authentication when making API requests on behalf of users.

GitHub Actions Tokens:
: For GitHub Actions workflows, you can use the GITHUB_TOKEN secret provided by GitHub. It's automatically available in your workflow environment.
: Use this token for authentication in your GitHub Actions workflows when interacting with your GitHub repository.

GitHub App Installations:
: Create a GitHub App in your GitHub account settings.
: Install the GitHub App on your repositories.
: Use the installation token provided by GitHub for authentication when making API requests as your GitHub App.

### Some 15 Github commands

Clone a Repository:
: To create a local copy of a remote repository on your machine.
```sh
git clone <repository_url>
```
Initialize a New Repository: 
: To start a new Git repository for a project.
```sh
git init
```
Add Changes to Staging Area: 
: To stage changes for the next commit.
```sh
git add <file>
```
Commit Changes: 
: To create a commit with staged changes.
```sh
git commit -m "Commit message"
```
Push to Remote Repository: 
: To upload local commits to a remote repository.
```sh
git push <remote_name> <branch_name>
```
Pull from Remote Repository: 
: To retrieve changes from a remote repository.
```sh
git pull <remote_name> <branch_name>
```
Create a New Branch: 
: To create a new branch for development.
```sh
git branch <branch_name>
```
Switch Branch: 
: To change your working branch.
```sh
git checkout <branch_name>
```
Merge Branches: 
: To integrate changes from one branch into another.
```sh
git merge <branch_name>
```
Fetch Remote Branches: 
: To retrieve information about remote branches.
```sh
git fetch
```
View Commit History: 
: To see a log of commit history.
```sh
git log
```
Create a Pull Request: 
: To propose changes and request them to be merged into a repository.
```sh
[Done On GitHub's website]
```
Review Pull Requests: 
: To review and comment on pull requests.
```sh
[On GitHub's website]
```
Accept Changes in a Pull Request: 
: To merge changes from a pull request.
```sh
[On GitHub's website or using `git merge`]
```
Create and Apply Stashes: 
: To temporarily save changes that are not ready to be committed.
```sh
git stash save "Stash message"
git stash apply
```

### 4 Github commmands that will be widly used
Git clone :
: the command will always copy to the local machine for users to have their own copy without directly changing in the main source

Git branch :
: to create a new branch for development and help developers perform their own changes without impacting eache others

Git add :
: this is to tell the git tool the the following files will be set to the stage status. this is one step of the developer to do to commit

Git commit: 
: this is to tell the tool that all that has been stage will be consololidated and this is the remarks/label to this commit

Git push: 
: This the step for the developer to put all the files from the committed stage to upload and fully commit to the repository
