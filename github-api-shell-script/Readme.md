# GitHub API User List with Shell Scripting

## Overview

This project is about creating a shell script that works with the GitHub API to list users who have read access to a specific repository.

## Script Details

The script `list-user.sh` is designed to be run from the command line. It requires the following parameters:

- `REPO_OWNER`: The owner of the GitHub repository.
- `REPO_NAME`: The name of the GitHub repository.

The script utilizes cURL to make HTTP requests to the GitHub API and jq for processing JSON responses.

## Usage

To use the script, follow these steps:

1. Clone the repository:

   ```bash
   git clone https://github.com/mohdaquib171/Shell-Scripting.git
   ```

2. Navigate to the directory containing the script:

   ```bash
   cd github-api-shell-script
   ```

3. Make the script executable:

   ```bash
   chmod +x list-users.sh
   ```

4. Run the script with the required parameters:

   ```bash
   ./list-users.sh <REPO_OWNER> <REPO_NAME>
   ```

Replace `<REPO_OWNER>` with the owner of the repository and `<REPO_NAME>` with the name of the repository.

## Example

```bash
./list-users.sh octocat Hello-World
```

This will list the users with read access to the "Hello-World" repository owned by "octocat".

## Notes

- Ensure you have a valid GitHub username and personal access token configured in the script for authentication.
- Ensure your personal access token has the necessary permissions to access the repository.
