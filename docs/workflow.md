# Git Workflow by Example

## Cloning the Repos

TODO

## Setup

The first thing you'll want to do is navigate to the direcory where the repository is stored. In my case that would be:
```
    cd ~/Git/3308project/minutes 
```

Next, I want to make sure that I am on the master branch and I want to get the latest changes that exist on the master branch
```
    git checkout master
    git pull origin master
```

In addition to this you may want to make sure that all branches are available to you. `git remote update` will fetch any branches that have been added to the remote repo. 

At this point any changes that have occurred on the master branch since my lst pull has been updated on my local machine's master branch. 

## Doing Work

It is important not to work directly on the master branch. In this example walkthrough I am just updating the `/minutes` repository, there is no code here to break, so I will be branching off of `master` to make changes here and in the `/milestones` repo. In the actual `/Wifiology` repo the only difference is that we will make our personal branches off of the `dev` branch. (more on this later in the doc)

So after I've done the setup steps above, I'm now ready to do some actual work.
First, I create the branch that I will work on and give it a descriptive title using `git branch your-branch-name` . In this case, I'm adding this git workflow document so I type.
```
    git branch add-git-workflow-docs
```

Now if I type `git branch` again I see the following printed in the terminal:
```
       add-git-workflow-docs
    *  master

```

The asterisk indicates that I am still on the `master` branch, before I do any work I want to switch to the feature branch using `git checkout branch-name`.
so,
```
    git checkout add-git-workflow docs
```

Then if I type `git branch` again I'll see the asterisk has moved to the branch that I want to work on. At this point this entire directory on my machine reflects the branch that I just created. If I change anything in this directory It will need to be added, commited, *and* pushed before any changes are saved remotely.

So at this point with half the doc written, I'll save my work and push it to just this branch on the remote repository.
