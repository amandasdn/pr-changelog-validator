# Changelog Validator GitHub Action

This repository uses GitHub Actions to check if the `CHANGELOG.md` files of projects are updated when code changes happen. The workflow checks if the changelog files in modified projects are updated and adds a comment to the pull request.

## How it works

1. **Find modified projects:** The workflow checks which projects were changed in the pull request.
2. **Validate changelogs:** It makes sure the `docs/CHANGELOG.md` file is updated for each modified project.
3. **Comment on the PR:** The workflow adds or updates a comment on the pull request, telling if the changelogs are updated or missing.

## Example output

### When changelog files were updated:
The PR comment will show:
![image](https://github.com/user-attachments/assets/a7d86b93-4328-4d8d-85f5-8739402fb693)

### When changelog files were not modified in the last commit
![image](https://github.com/user-attachments/assets/c371ea50-3b24-4a4c-ae7e-ca5545ab9f2a)
