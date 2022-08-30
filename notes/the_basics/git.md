# git
git is a free open source version control system.

The basic flow of git goes:

1. Create a "repository" (project) with a git hosting tool (like Bitbucket or Github)
        
2. Copy (or clone) the repository to your local machine

    `git clone <ssh repo link here>`

3. Add a file to your local repo and "commit" (save) the changes
    `echo "Earth's moon" >> new_file.txt`

    `git status`

    This will add it to a staging area in local machine
    
    `git add new_file.txt`

    This adds a commit with a message

    `git commit -m 'initial file'`


4. "Push" your changes to your main branch. The commits are now on the remote repo(origin)

    `git push origin main`

5. "Pull" the changes to your local machine from remote repo (origin)
    ` git pull --all`

6. Create a "branch" (version) called `DE-388`, make a change, commit the change
    `git branch DE-388`

    switch to the branch to use it

    `git checkout DE-388`

    `git add station.txt`

    `git commit -m 'add new station file'`


7. Open a "pull request" (propose changes to the main branch)

8. "Merge" your branch to the main branch
    `git status`

    `git checkout main`

    `git merge DE-388`

9. Delete the `DE-388 branch` as you don't plan on using it anymore

    `git branch -d DE-388`

    `git status`


# fetch

1. fetching all remote branches

    `git fetch --all`

    fetch specific branch

    `git fetch <remote> <branch>`

2. Fetch remote brnach

    `git remote add coworkers_repo git@bitbucket.org:coworker/coworkers_repo.git`

    `git fetch coworkers_repo coworkers/feature_branch`

    `git checkout coworkers/feature_branch`

    Here we have created a new local branch named local_feature_branch. This puts updates HEAD to point at the latest remote content and we can continue development on it from this point.
    
    `git checkout -b local_feature_branch`







