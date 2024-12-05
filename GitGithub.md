### Git

#### 1. What is Git?
Git is a distributed version control system that allows multiple developers to work on a project simultaneously. It tracks changes in files, enabling collaboration, history tracking, and version control.

#### 2. What is the difference between Git and GitHub?
- **Git**: A version control system that helps track changes in your code locally on your computer.
- **GitHub**: A cloud-based platform for hosting and sharing Git repositories. It provides a collaborative environment for version control and project management.

#### 3. What are Git commands used for version control?
- `git init`: Initializes a new Git repository.
- `git clone`: Clones a remote repository to your local machine.
- `git add`: Stages changes for the next commit.
- `git commit`: Records the changes made to the repository.
- `git push`: Uploads your local commits to a remote repository.
- `git pull`: Fetches and merges changes from a remote repository to your local repository.
- `git status`: Displays the state of the working directory and staging area.
- `git log`: Shows the commit history.

#### 4. What is a branch in Git?
A branch in Git is a separate line of development that allows you to work on features or fixes without affecting the main codebase. Common branches include `main` (or `master`) and feature branches.

#### 5. What is a commit in Git?
A commit in Git is a snapshot of your project at a specific point in time. It contains changes that have been recorded to the version history of the repository.

#### 6. What is a merge in Git?
Merging in Git involves combining the changes from different branches into one. A merge can be performed using the `git merge` command.

#### 7. What is a conflict in Git?
A conflict in Git occurs when two branches make changes to the same part of a file. Git cannot automatically decide which changes to keep, and you must manually resolve the conflict.

#### 8. What is the use of `.gitignore`?
The `.gitignore` file is used to specify files and directories that should not be tracked by Git, such as temporary files, build outputs, and sensitive information.

#### 9. What is a pull request in GitHub?
A pull request is a method for submitting contributions to a project. It allows you to propose changes to a repository, and once reviewed, the changes can be merged into the main branch.

#### 10. What is a fork in GitHub?
A fork is a copy of a repository that allows you to make changes without affecting the original project. It is commonly used when contributing to open-source projects.

#### 11. What is a remote repository in Git?
A remote repository is a version of your project that is hosted on the internet (such as GitHub, GitLab, or Bitbucket). It allows multiple users to collaborate on the project.

#### 12. What is a tag in Git?
A tag is a reference to a specific commit, often used to mark a release or important point in the history of a project.

#### 13. What is the `git rebase` command?
The `git rebase` command is used to integrate changes from one branch into another by applying the changes in a linear sequence. It is used to maintain a clean commit history.

#### 14. What are Git submodules?
Git submodules allow you to include one Git repository inside another. This is useful for managing dependencies or libraries as separate repositories within a main project.

---

### GitHub

#### 15. What is GitHub?
GitHub is a web-based platform that hosts Git repositories, enabling version control, collaboration, and project management. It provides features like issue tracking, pull requests, and continuous integration.

#### 16. What are GitHub Actions?
GitHub Actions is a feature that allows you to automate workflows, such as building, testing, and deploying code. It is commonly used for Continuous Integration and Continuous Deployment (CI/CD).

#### 17. What is the difference between `git pull` and `git fetch`?
- **`git pull`**: Fetches changes from the remote repository and automatically merges them into your local repository.
- **`git fetch`**: Fetches changes from the remote repository without merging them, allowing you to review the changes before merging.

#### 18. What is a GitHub Gist?
A GitHub Gist is a simple way to share code snippets, notes, or documents. Gists can be public or private and can be shared easily across platforms.

#### 19. What is the `git reset` command?
The `git reset` command is used to undo changes by resetting the current state of the repository to a previous commit. It has different modes like `--soft`, `--hard`, and `--mixed` to control the scope of the reset.

#### 20. What is a collaborator in GitHub?
A collaborator is a person who has access to a repository and can contribute to it. They can clone the repository, push changes, and review pull requests, depending on their permissions.

#### 21. What is a GitHub organization?
A GitHub organization is a shared account that allows multiple users to collaborate on repositories and manage permissions in an organized way, suitable for teams and enterprises.

#### 22. What is the use of GitHub Pages?
GitHub Pages is a service that allows you to host static websites directly from a GitHub repository. It is commonly used for personal projects, documentation, and portfolios.

#### 23. What is the difference between `git push` and `git pull`?
- **`git push`**: Uploads local commits to the remote repository.
- **`git pull`**: Downloads changes from the remote repository to your local machine and merges them with your working files.
