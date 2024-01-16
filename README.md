# github-codecommit
## Sync with AWS CodeCommit

This GitHub Actions workflow is designed to sync your GitHub repository with AWS CodeCommit. It triggers on every push to the `main` branch.

## Workflow Details

### Trigger
The workflow is triggered on a `push` event to the `main` branch.

```yaml
on:
  push:
    branches:
      - main
```
## Job: sync
This workflow has a single job named sync, which runs on the latest version of Ubuntu.

# Usage
1. Set up the required AWS credentials as secrets in your GitHub repository (AWS_ACCESS_KEY_ID and AWS_SECRET_ACCESS_KEY).
2. Copy and paste the provided YAML code into your GitHub Actions workflow file (e.g., .github/workflows/sync-with-aws-codecommit.yml).

Now, every push to the main branch will trigger this workflow, syncing your GitHub repository with the specified AWS CodeCommit repository.
