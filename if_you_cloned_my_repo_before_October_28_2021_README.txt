# If you cloned one of my repositories before I switched all from "master" to "main" branches 
# (October 28, 2021), you will have to make a couple of changes on your side as well:

# From https://hackernoon.com/how-to-rename-your-git-repositories-from-master-to-main-6i1u3wsu

# Switch to the "master" branch:
git checkout master

# Rename it to "main":
git branch -m master main

# Get the latest commits (and branches!) from the remote:
git fetch

# Remove the existing tracking connection with "origin/master":
git branch --unset-upstream

# Create a new tracking connection with the new "origin/main" branch:
git branch -u origin/main
