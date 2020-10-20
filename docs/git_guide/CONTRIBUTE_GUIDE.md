---
layout: default
title: ContributeGuide
parent: Git Guide
nav_order: 2
---

# Contributor Guide

If you are new to collaborating through GitHub, there may be some awkward or difficult parts, but the more comfortable you are, the better you will learn.

To make your first contribution, just follow the simple steps below.

<img align="right" width="300" src="https://raw.githubusercontent.com/hanssak/hanssak.github.io/tmp/docs/git_guide/repo/fork.png" alt="This repository Fork" />

If you do not have Git right now, please [Install](https://help.github.com/articles/set-up-git/).

## Fork the repository

Fork this repository by clicking the Fork button at the top of this page. This will create a replica of this repository in your account.

## Cloning the repository

<img align="right" width="300" src="https://raw.githubusercontent.com/hanssak/hanssak.github.io/tmp/docs/git_guide/repo/clone.png" alt="This repository Duplicate" />

Now clone this repository to your computer. Click the Duplicate button and click the Copy to Clipboard icon.

Open a terminal and run the following Git command:

```
git clone "address just copied"
```

"The address you just copied" (without the quotes) is the address of this repository. Refer to the previous steps to get the address.

<img align="right" width="300" src="https://raw.githubusercontent.com/hanssak/hanssak.github.io/tmp/docs/git_guide/repo/copy-to-clipboard.png" alt ="Copy URL to clipboard" />

example:

```
git clone https://github.com/your_id/OpenNetLink.git
```

`your_id` is your GitHub account. Here on GitHub
Copy the contents of the OneNetLink repository to your computer.

## create branch

If it's not already in the repository directory, go there

```
cd OpenNetLink
```

Now create a branch using the `git checkout` command.

```
git checkout -b <add_your_id>
```

example:

```
git checkout -b add_johndoe
```

(You don't have to include *add* in the branch name.
However, since the purpose of this branch is to add your name to the list, it makes sense to include *add* in the name.)

## Make the necessary changes and commit

Now open the `CONTRIBUTORS.md` file in a text editor and edit it.
Please refer to this [cheat sheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) for how to use Markdown.

Add the following information to the end of `CONTRIBUTORS.md`.

```
-[your-name](https://github.com/your_id)
```

example:

```
-[John Doe](https://github.com/johndoe)
```

Please note that there is no space between `](`. Save the file and exit.

You can see the changes by running the `git status` command in your project directory. Add the changes with the `git add` command below.

```
git add CONTRIBUTORS.md
```

Now commit the changes with the `git commit` command below.

```
git commit -m "Add <your_id> to Contributors list"
```

Replace `<your_id>` with your github account.

## Push your changes to GitHub

Push the changes with the `git push` command.

```
git push origin <add_your_id>
```

Replace `<add-your-name>` with the name of the branch you created earlier.

## Submit changes for review

If you go to your repository on GitHub, you can see the `Compare & pull request` button. Click that button.

<img style="float: right;" src="https://raw.githubusercontent.com/hanssak/hanssak.github.io/tmp/docs/git_guide/repo/compare-and-pull.png" alt="Pull request Create" />

Now submit your pull request.

<img style="float: right;" src="https://raw.githubusercontent.com/hanssak/hanssak.github.io/tmp/docs/git_guide/repo/submit-pull-request.png" alt="Submit a pull request"/>

Now, after I check your changes, you will receive a notification email when merging to the master branch.
