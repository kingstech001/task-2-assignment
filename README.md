# Version Control
     Version control is a system that allows you to track and manage changes to files over time. It is essential for:
  + Collaboration: Multiple team members can work on the same project.
  + History Tracking: Allows you to see what changes were made, when, and by whom.
  + Reverting Changes: Enables undoing mistakes by rolling back to previous versions.


# Difference Between Git and GitHub

  ## Git
     Git is a distributed version control system that tracks changes in your source code during development. It enables you to manage your code history, create branches, merge code, and collaborate with others efficiently, all locally on your computer. Git is a tool for developers to save, manage, and revert code changes without relying on an internet connection.

   ### Key Features of Git:
   + Tracks code changes over time.
   + Allows multiple developers to work on the same project simultaneously.
   + Enables creation of branches for testing new features.
   + Works entirely offline


   ## GitHub
     GitHub is a cloud-based platform for hosting Git repositories and enabling collaboration. It acts as a remote repository for your Git projects, making it easy to share your code, review others' work, and manage team contributions. GitHub also adds features like issue tracking, pull requests, and continuous integration (CI) to facilitate modern software development workflows.

   ### Key Features of GitHub:
   + Provides a remote storage location for Git repositories.
   + Offers tools for code review, issue tracking, and project management.
   + Enables collaboration with teammates in real-time.
   + Integrates with various tools and CI/CD pipelines.


# GitHub Alternatives
 + GitLab
 + Bitbucket
 + SourceForge


# Difference Between git fetch and git pull

 ## git fetch
     It downloads changes (commits, branches, tags, etc.) from the remote repository to your local repository without merging them into your working directory.

   ### Use Case:
     When you want to see what changes are available in the remote repository without affecting your current work.


 ## git pull
     Combines the functionality of git fetch and git merge. It downloads changes from the remote repository and immediately merges them into your current branch.

   ### Use Case:
     When you're ready to integrate remote changes directly into your local branch.

# git rebase
  In simple terms, git rebase is a way to move your changes (commits) to a new base branch, making your commit history cleaner and more linear. It helps in keeping your project's history tidy, especially when working with teams.

   ## How It Works:
      Imagine you created a feature branch (feature) based on the main branch. While working on your feature, others made changes to main. If you want your feature branch to include the latest updates from main without creating a merge commit, you can use git rebase.
   ### Command for git rebase
     Switch to the branch you want to rebase:

   #### Switch to the branch you want to rebase:
      git checkout feature

   #### Rebase your branch onto the updated branch (e.g., main):
      git rebase main

   #### If there are conflicts, Git will pause the rebase, and you’ll need to resolve them. After resolving:
      git add .
      git rebase --continue

   #### Once done, push your rebased branch:
      git push --force

