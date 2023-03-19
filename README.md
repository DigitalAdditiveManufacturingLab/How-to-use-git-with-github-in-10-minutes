# How to Use Git with GitHub
Git is a powerful version control system that allows you to manage and collaborate on code. GitHub is a web-based hosting service for Git repositories, which provides a range of tools for managing and collaborating on code. DO NOT USE `add-commit-push` ON SHARED REPOSITORIES!!!

# Forking and creating a new local branch
To get started, you will need to fork the repository on GitHub that you want to work on. To do this, navigate to the repository's page on GitHub and click the "Fork" button in the top right corner. This will create a copy of the repository in your own GitHub account.

Next, clone the repository to your local machine using the command `git clone <repository-url>`. This will create a local copy of the repository on your machine.

Create a new local branch for your changes using the command `git checkout -b <branch-name>`. This will create a new branch and switch to it. You can now make changes to the code and commit them to your local branch using the command `git commit -m "<commit-message>"`.

# Updating the main branch
If the main branch of the repository is updated while you are working on your local branch, you will need to update your local branch with the latest changes before you can merge your changes into the main branch.

To update your local branch, switch to the main branch using the command `git checkout main`. Then, run the command `git pull` to download the latest changes from the main branch on GitHub. This will update your local main branch with the latest changes.

Next, switch back to your local branch using the command `git checkout <branch-name>`. Then, merge the changes from the main branch into your local branch using the command `git merge main`. This will merge the changes from the main branch into your local branch.

# Solving merge conflicts
If there are conflicts between your changes and the changes in the main branch when you update your local branch, you will need to resolve these conflicts before you can merge your changes into the main branch.

To resolve merge conflicts, first update your local main branch with the latest changes on GitHub using the `git pull` command. Then, switch back to your local branch using the command `git checkout <branch-name>`.

Next, run the command `git merge main` to merge the changes from the main branch into your local branch. This will identify any conflicts between your changes and the changes in the main branch.

Open the files with conflicts in a text editor and look for the conflict markers `<<<<<<<`, `=======`, and `>>>>>>>`. Edit the files to resolve the conflicts, then save the files.

Once you have resolved the conflicts, add the changes to your local branch using the command `git add <file-name>`. Then, commit the changes to your local branch using the command `git commit -m "<commit-message>"`. You can now push the changes to your GitHub account and create a new pull request to merge your changes into the main branch of the repository.

# Using pull requests to merge
Once you have made your changes and committed them to your local branch, you can use a pull request to merge your changes into the main branch of the repository.

To create a pull request, first push your local branch to your GitHub account using the command `git push -u origin <branch-name>`. Then, navigate to the repository's page on GitHub and click the "New pull request" button. Select your branch from the dropdown menu, enter a brief description of your changes, and click the "Create pull request" button.

Your pull request will now be reviewed by the repository's maintainers, who may suggest changes or request further information. Once your changes have been approved, you can merge your changes into the main branch of the repository.

# Merging a pull request with squash and merge
When merging a pull request, you can choose to use squash and merge to combine all of the commits in the pull request into a single commit on the main branch. This can help to keep the main branch clean and organized.

To use squash and merge, first navigate to the pull request you want to merge on the GitHub website. Click the "Merge pull request" button, then select "Squash and merge" from the dropdown menu. Enter a commit message for the merged changes, then click the "Confirm squash and merge" button.

This will combine all of the commits in the pull request into a single commit with the commit message you entered. The changes will now be merged into the main branch of the repository.

# Deleting the local branch
After your changes have been merged into the main branch of the repository, you should delete the local branch that you created for your changes.

To delete a local branch, first switch to another branch using the command `git checkout <other-branch>`. Then, run the command `git branch -d <branch-name>` to delete the local branch you want to delete.

# Synchronizing the local main branch
After your changes have been merged into the main branch of the repository, you should synchronize your local main branch with the latest changes on GitHub.

To synchronize your local main branch, first switch to the main branch using the command `git checkout main`. Next, run the command `git pull` to download the latest changes from the main branch on GitHub. This will update your local main branch with the latest changes.



