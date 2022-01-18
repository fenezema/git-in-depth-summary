# (Section 1) Git - That One Friend/Foe You Interact with Everyday

## Git References
Git has a few references on its workflow in general. In an oversimplification, there are: Head, Branches, Tags, Annotated Tags.

### HEAD
We can think Head like a symlink. If you're not familiar with Symlink, you can this [article](https://www.freecodecamp.org/news/symlink-tutorial-in-linux-how-to-create-and-remove-a-symbolic-link/) about symlink.

A symlink is simply a referer to another thing, in Unix/Unix-like OS, a symlink is simply a referer to another directory or file.

So, you can think that HEAD is like a symlink, that pointed out on the current commit (or branches, that will be explain in this section later) we are currently on. 

**NB : to check current HEAD commit, we can use this command `git rev-parse head` and it will print out the commit SHA1 in our terminal**

### Branches
Branch(es) is simply another commit to begin with. 
But in a workflow topic, a branch is, like what its name, a branch, of the current commit. A brief of explanation for this is that, when we're doing a collab works, we want to work together, but not that very together-y, in a sense that, if it too dependent to one another, if it will possibly take more times to develop because of the nature of wait and hold.

Mainly because, let's say that developer Fabs is working on Feature A, while developer Basse is working on Feature B. They want to work together, but separate at the same time, so every developer can do concurrent works without interupting the work of other developer in their own seperate branches. So everyone has a copy of that repo without interupting the others. In the end, after every developer get their shots done, their branches can be merge into the main/master branch.

We can create a new branch by typing this particular command on our holy terminal

`git branch -b <branch name>`

This command will create a new branch with the parent commit of the current commit/HEAD for that matters. 