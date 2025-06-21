# github-actions-test
GitHub Actions practice - Can we curl a file and commit it to a branch upon PR?

## Overview

This repository demonstrates how to use GitHub Actions to automate the following workflow when a pull request (PR) is submitted:

1. **Trigger on PR submission**
2. **Curl an image from a public URL**
3. **Commit the image to the PR branch**
4. **Merge the PR**
5. **Close the PR**

> **Note:** This project is a work in progress and not yet functional.

## Planned Setup Steps

1. **Create a GitHub Actions Workflow**
    - Add a workflow YAML file in `.github/workflows/`.
    - Configure it to trigger on `pull_request` events.

2. **Curl the Image**
    - Use a step in the workflow to download the image:
    - URL: [Sample Image](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSFUAfyVe3Easiycyh3isP9wDQTYuSmGPsPQvLIJdEYvQ_DsFq5Ez2Nh_QjiS3oZ3B8ZPfK9cZQyIStmQMV1lDPLw)
    - Save the image to the repository.

3. **Commit the Image**
    - Configure the workflow to commit the downloaded image to the head branch of the PR.

4. **Merge the PR**
    - Set up a workflow step (or use a bot) to automatically merge the PR after the image is committed.

5. **Close the PR**
    - Ensure the PR is closed after merging.

## To Do

- [ ] Create initial workflow file
- [ ] Implement image download step
- [ ] Automate commit to PR branch
- [ ] Automate PR merge and closure
