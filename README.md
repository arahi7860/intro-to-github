# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) SOFTWARE ENGINEERING IMMERSIVE

## Intro to GitHub

### Lesson Objectives

GitHub is one of the backbones of the industry. It will become one of your most-visited websites in no time, so let's use our work from the Intro to Git Lesson to explore it a little more.

By now, you've surely heard all the GitHub keywords– local versus remote repositories; forking, cloning, branching, and stashing; pull requests, merging, and merge conflicts; issues; wikis; projects; tags, shields...

By the end of this lesson, you will be a little more comfortable with:

- The GitHub user interface.
- Forking and cloning a remote repository.
- Syncing local and remote repositories.
- Collaborating with teams and colleagues on the same project.
- Merging branches and pull requests.
- Handling merge conflicts.

<br>

### Overview

We've already learned about git and created a local repository, but what about a remote repository?

#### Remote Repositories

![Alt Text](https://media.giphy.com/media/3orifhOeMIcO6YE0fu/giphy.gif)

A remote repository is just another repository, but it doesn't live on your computer, like your local repository. Depending on your permissions, you can push code up to it and pull code down from it.

<br>

#### Introducing GitHub

At its core, remote repositories are cloud backups of our code.

Comparable to cloud storage apps like Google Drive, Microsoft OneDrive, and DropBox, there are alternatives to GitHub, but GitHub has become the most commonly used because of its stellar graphical interface and useful collaboration features.

For these reasons, it's become integral to collaboration, and most software engineering teams depend on it.

<br>

### Code Along, Part 3

#### Create a Remote Repository

- Open your GitHub Enterprise.
- Click the plus sign in the menu and select "new repository." _What does the new repo screen allow you to do?_
- For consistency, we'll enter the same name that we used for our local version– `mean-girls`.

#### Connect Your Local Repository

Once you create a new remote repository, you'll see this screen:

![mg1](https://user-images.githubusercontent.com/6153182/33035113-09f033dc-cdf8-11e7-8f7a-24fda5b84a2c.png)

We already have our local repository, so we'll use the third option, "push an existing repository from the command line."

- Copy the two lines under this option.
- Open Terminal, and confirm you're in the correct repo with `pwd`.
- First, run `git remote -v`. _What does it say?_
- Now paste the commands into terminal and hit enter. _What did these commands do?_

### Boom. Connected.

<br>

***

### Some Explanations

#### Forking

A fork is a _copy_ of a repository. Forking a repository allows you to freely experiment with changes without affecting the original project. Forks are used to either propose changes to someone's project or to use someone's project as _starter code_ for your own idea.

![fork](https://user-images.githubusercontent.com/6153182/33048606-bed6d2c0-ce29-11e7-8f54-bf7cf4560dec.png)

#### Cloning

When you create a repository on GitHub, it exists as a remote repository. You can clone your repository to create a local copy on your computer and sync between the two locations.

![clone](https://user-images.githubusercontent.com/6153182/33048675-24e2bc50-ce2a-11e7-804f-634a7790107c.png)

#### Pull Requests

Pull requests let you notify others about changes you've pushed to a branch in a repository on GitHub. Once a pull request is opened, you can discuss and review the potential changes with collaborators and add follow-up commits before your changes are merged into the base branch.

### [Pull Request Tutorial](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request)

![bridgid](https://user-images.githubusercontent.com/6153182/33048688-3098920e-ce2a-11e7-9873-29cc04f36d49.png)

#### Pulling

Each of you should now have updated code on GitHub, but your local Git repo
will be behind.  We need to get the latest code off of GitHub.  We can do this
by pulling the changes that we merged. Git pull is a combination of git fetch and git merge. The command to do this is:

`git pull`

This gets the latest copy of our code from the master branch of our original
repository.

#### Merge Conflicts

Sometimes, if the same file has been edited on multiple different collaborators' local copies, attempting a PR or pulling their code will create a _merge conflict_. Let's not worry about that for now– we'll return to discuss it in Unit 3, when we have a group project to test this all out. 

<br> 

***

### Recap

Your most common git flow will look like this:

- `fork`
- `clone`
- Make changes to a file.
- `git add <filename>` or `git add .`
- `git commit -m "with a commit message"`
- `git push <remote name> <branch name>`
- Then go to GitHub and `create pull request`.

What does this all look like, visually? Let's check out the _tree_ using GitKraken, a desktop client.

<br>

***

### Want more practice?

<details><summary>Self Guided Learning</summary>

<br>

![Alt Text](https://media.giphy.com/media/xT9KVtQBk8cGFcZH4A/giphy.gif)

The last time we saw the Mean Girls, Regina was kicked out. Let's add Karen to take her place:

- Create a `karen.txt` file and add: `"There's a 30% chance that it's already raining"`.
- Add, commit, and push this file to GitHub.

#### Add Tina Fey (last Mean Girls reference, I promise :grimacing: )

Tina Fey is here to teach us about forking, cloning, and pull requests!

![Alt Text](https://media.giphy.com/media/3o7aTLkyh3yAG6DEuQ/giphy.gif)

Now, working with a partner, follow the above examples just did and take turns: (Example names: Ruben & Leah)

- Ruben should fork and clone Leah's repo
- Add your-name.txt and add your "catchphrase" to the text inside
- Ruben should create a pull request
- Leah  should accept this pull request and merge it into her GitHub repo
- Leah should pull the new changes Ruben made (via using the terminal)

and vice versa.

</details>
