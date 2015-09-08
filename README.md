https://github.com/ivanjfernandez1/Adding-to-Git.git
Adding a file to a repository from the command line

You can upload an existing file to a GitHub repository using the command line.

While you can add a new file to a repository from the GitHub website, you may have an existing file you'd like to include in your repository.

This procedure assumes you've already:

    Created a repository on GitHub, or are a collaborator on someone else's repository.
    Cloned the repository locally on your computer


For more information, see "Remove sensitive data."

    On your computer, move the file you'd like to upload to GitHub into the local directory that was created when you cloned the repository.

    Open Terminal (for Mac users) or the command prompt (for Windows and Linux users).

    Change the current working directory to your local repository.

    Stage the file for the first commit to your repository.

    git add .
    # Adds the files in the local repository and stages them for commit. To unstage a file, use 'git reset HEAD YOUR-FILE'.

    Commit the files that you've staged in your local repository.

    git commit -m 'First commit'
    # Commits the tracked changes and prepares them to be pushed to a remote repository. To remove this commit and modify the file, use 'git reset --soft HEAD~1' and commit and add the file again.

    Push the changes in your local repository to GitHub.

    git push origin master
    # Pushes the changes in your local repository up to the remote repository you specified as the origin

