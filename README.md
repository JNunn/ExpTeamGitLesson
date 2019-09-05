# ExpTeamGitLesson

A test ground for YNAP Experience team members to try out git.

Go wild! Make changes, commit your changes, push them from your local repository to the remote, and pull your teammates changes to merge into yours!

The world is your oyster.

## commands

First up, open your Git GUI - Sourcetree is one recommendation of a Git GUI you could use here. Or, if you are feeling brave, open your machine's command line and run the commands directly into that. The latter is not as visually friendly but does the same job.

Direct to the folder that you'd like to copy the remote repository into:

```
cd <yourdirectory>
```

Copy the repository folder to this local folder:

```
git clone git@github.com:JNunn/ExpTeamGitLesson.git
```

Now that you should have the files appearing locally on your machine, point your machine to look at this new local project folder:

```
cd <ExpTeamGitLesson>
```

If you open the index.html file in your browser you will see it come to life. Try making a change to the local files and see what happens when you refresh the browser. To see what changes you have made, run the following:

```
git status
```

Once you have made some changes that you'd like to share, the changes need to be committed and pushed back up to the remote repository. Make sure to add all changes using '.' and to leave a message to document what has changed using '-m':

```
git add .
git commit -m”This is my update”
git push
```

If a teammate has also made some changes and pushed them to the remote repository, you may want to pull these down to merge into your local version:

```
git pull
```

If many people are working on a project, or you have many features to develop, you may want to introduce some branches to your repository:

```
git checkout -b <branchname>
git push —set-upstream origin <branchname>
```

This is basically saying:

- checkout a new branch locally called a specific name
- push that branch to the remote repository
- while pushing it to the remote repository, set the local branch to track it's remote counterpart (it will push and pull to this automatically)

## git file

A git project will have an automatically generated '.git' folder within it. Pay particular attention to the config file within this folder to check useful information, for example, whether the location of your remote repository is correct.
