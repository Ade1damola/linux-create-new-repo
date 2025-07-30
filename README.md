 # linux-create-new-repo 

This script creates a new GitHub repository using the GitHub API (via curl) and initializes a local Git repository with a README.md, then pushes it.

## Prerequisites 
To use this script, ensure you have the following installed and configured:
1. Git: Command-line version control system.
- Check with: `git --version`
2. jq: A lightweight and flexible command-line JSON processor.
This is used to parse responses from the GitHub API.
- Check with: `jq --version`
- Install example:
    + `sudo apt-get install jq` on Debian/Ubuntu
    +  `brew install jq` on macOS
    +  https://geeksforgeeks.org/git/how-to-install-jq-in-git-bash/ on Git Bash for Windows
3. GitHub Personal Access Token (PAT):
You need a PAT with 'repo' scope (full control of private repositories).
- Generate one here: https://github.com/settings/tokens/new



## Steps
- Clone the repository
  ```bash
  git clone https://github.com/Ade1damola/linux-create-new-repo.git
  ```

- Make the script executable
  ```bash
  chmod u+x newGithubRepo
  ```

- Run the script
  ```bash
  ./newGithubRepo
  ```
- You can now navigate into the '$repoName' directory and start working
  ```bash
  cd $repoName
  ```
