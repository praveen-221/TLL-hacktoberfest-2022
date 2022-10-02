# Contributing

Before working on a new feature or fix, please let everyone know so we don't work on the same issues. Please create an issue and assign yourself in the [Issues tab](https://assets.digitalocean.com/articles/hfestfirstpr-pr.gif).

# How to run the project locally

1. fork and clone the repository
2. `yarn install` in the root folder to install dependencies, which will install dependencies in both client and server
3. `yarn start` to start both client and server
   `yarn client` to start client only
   `yarn server` to start server only

The frontend is run on port 5173 and backend is run on port 4002.

# Installing packages
in the root folder, 
frontend/client: `yarn workspace client add <package>`
backend/server: `yarn workspace server add <package>`

or navigate to the respective folder and `yarn add <package>`

# Fetch new changes from upstream

### From terminal

**1.** If anyone contribute to this repository, then the changes will not reflect in your local repository. For that:

**2.** Setup a reference(remote) to the original repository to get all the changes from the remote.

```
   git remote add upstream https://github.com/webdev-20/TLL-hacktoberfest-2022.git
```

**3.** Check the remotes for this repository.

```
   git remote -v
```

**4.** Fetching from the remote repository will bring in its branches and their respective commits.

```
   git fetch upstream
```

**5.** Make sure that you're on your main branch.

```
   git checkout main
```

**6.** Now that we have fetched the upstream repository, we want to merge its changes into our local branch. This will bring that branch into sync with the upstream, without losing our local changes.

```
   git merge upstream/main
```

**7.** Or you can club step 4th and 6th together using:-

```
   git pull upstream main
```

### From github website

[![](https://i.imgur.com/7eLUTJQm.jpg)](https://i.imgur.com/7eLUTJQ.png)

Update the branch and then go to the project folder in terminal and pull the changes to your local repository
```
   git pull
```

# Creating a Pull Request

1. [Fork](https://docs.github.com/en/get-started/quickstart/fork-a-repo) the repository
2. [Clone](https://docs.github.com/en/get-started/quickstart/fork-a-repo#cloning-your-forked-repository) to your local machine
3. Create a new branch `git checkout -b branchname`, example of a branch name
   - feature/nav
   - fix/header
   - chore/some-chores
4. Edit locally
5. Stage changes and commit <br/>
   `git add .` <br/>
   `git commit -m "commit message"` <br/>
   `git push origin feature/nav`
6. Go to your forked repo and click on "Open Pull Request" on the top banner where it says "The branch is x commits ahead of ..."
   [![](https://i.imgur.com/luSAAVKm.jpg)](https://i.imgur.com/luSAAVK.png)

Read more: <br/>
https://docs.github.com/en/get-started/quickstart/contributing-to-projects <br />
https://www.digitalocean.com/community/tutorials/hacktoberfest-how-to-submit-your-first-pull-request-on-github

<br />

# Reviewing a Pull Request

If reviewing (optional), [install GitHub CLI](https://cli.github.com/) and ask to be added to the Code Review team.
