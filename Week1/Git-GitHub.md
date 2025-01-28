*Feel free to explore this document and the linked resources (as well as other documentation on these tools) to help understand how different environments work. I encourage you to come back to it later as you get experience and start to understand more about the differences once you have more experience and context...*

# Git & GitHub

## Git
Git is a versioning software that sits on your local computer and aids in the tracking of changes for **code files**. You'll need to [download Git] on your computer.

## GitHub
[GitHub] is a website that hosts remote repositories (read: repos) that hold an enitre project's folders, files, and version history for each file. Repos can be private or public, meaning only you can see them or anyone on the internet can see everything in the repo, respectively. 

You can check out the [GitHub documentation] for more info about GitHub... it's pretty user friendly!

You can interact with GitHub in 3 ways: CLI (command line interface), the website, and the GitHub Desktop app. 

When you intereact with GitHub, you're usually connecting your local repo (on your computer) and the remote repo (on GitHub) in some way. Here are several basic terms you'll use when to getting started:

### GitHub Jargon to Get Started
- [add] - specifies which files you want to be commited - you really only use this when you're using the CLI
- [commit] - saves a change you've made to the respective branch you're in (either the main or a side branch), a commit acts as a snapshot of the file at the time of the commit
- [push] - updates the repote repo with the changes made locally
- [pull]- gets the most recent version of the remote repo to your local repo
- [branch] - a version of your project where you are making changes (like adding a new feature) but not changing the base branch. This is helpful if you want to try something out without accidentally messing up your main branch.
- [pull request] - propose changes to a repo, a pull request is made in a branch, so it does not affect the base branch until approved
- [merge] - updates the base branch with the updates proposed in a pull request
- [fork] - a copy of a repo on your own account, changes can be made to this new forked copy without affecting the original repo (unless you submit a pull request and they accept it!), any changes made to the original branch can be pulled to your fork
- [clone] - copies your remote repo to your local machine
- [fetch upstream] - gets all the new changes from the remote repo (or original repo, in the case of a forked repo) without merging

### Use Cases
Let's say you have a repo set up for an app you're builidng and just added a developer to help you build out the app. You have a public remote repo already set up, but since it is your project, only you have permissions to make changes to it.

#### Use Case 1: Bug fix
You need to fix a bug you've recently discovered in your app. You assign your new developer to fix the bug. 

    They will:

        1. Fork the project repo to their GitHub account and clone it to their local computer.
        2. Make the changes to the code to fix the bug. 
        3. Add, commit, and push the changes to their forked branch of the repo.
        4. Submit a pull request to add the changes to your original repo.

    Then, you will:
    
        1. Review the changes and decide whether they are sufficient to fix the bug and haven't affected anything else.
        2. If they pass your assessment, you can merge these changes to the base or main branch.

#### Use Case 2: Adding a new feature
You want to build out a new "share" feature in your app without affecting the functionality of the existing code. 

    You will:

        1. Pull the most recent version of the remote repo to your local - you want that updated bug fix!
        2. Create a new branch to build out the new feature. We'll name it "add-share-feature". 
        3. Build and test your new feature code on the "add-share-feature" branch. You add, commit, and push your changes to this branch.
        4. When your new feature is complete, you can create a pull request to merge your "add-share-feature" branch to the main branch.
        5. After doing a final review, you can merge your branches and your new feature will be added to your main branch.

_____________________________
# Next Steps:
- Make sure you have Git installed on your computer (run `git --version` in a terminal) or download git if needed​

- Use the linked documentation to set up a GitHub account and local connection​

- Fork the Spoon-Knife repo, make a change locally, and (add, commit, and) push it to your repo​

[download Git]: https://git-scm.com/downloads
[GitHub]: https://github.com/
[GitHub documentation]: https://docs.github.com/en/get-started/using-git/about-git

[add]: https://github.com/git-guides/git-add
[commit]: https://docs.github.com/en/get-started/quickstart/create-a-repo#commit-your-first-change
[push]: https://docs.github.com/en/get-started/using-git/pushing-commits-to-a-remote-repository
[pull]: https://docs.github.com/en/get-started/using-git/getting-changes-from-a-remote-repository#pulling-changes-from-a-remote-repository
[branch]: https://docs.github.com/en/get-started/quickstart/github-flow#create-a-branch
[pull request]: https://docs.github.com/en/get-started/quickstart/github-flow#create-a-pull-request
[merge]: https://docs.github.com/en/get-started/quickstart/github-flow#merge-your-pull-request
[fork]: https://docs.github.com/en/get-started/quickstart/fork-a-repo
[clone]: https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository
[fetch upstream]: https://docs.github.com/en/get-started/using-git/getting-changes-from-a-remote-repository#fetching-changes-from-a-remote-repository
