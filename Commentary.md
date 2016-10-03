## Part 1:

Each of us makes changes to our local copy of the repo, and then pushes to remote. Then the other person pulls down the recent changes/commits, makes their own additions (that create no conflicts), and pushes to master. We repeat this for a bit.

## Part 2:

We get a conflict because there are remote changes that I haven't saved locally. User B can resolve this conflict by pulling before pushing.

## Part 3:

Since User A never pushes to remote, User B can push their changes without a conflict.

## Part 4:

When User A tries to push to master, they get a merge conflict resulting from the work of User B in Part 3. When User B tries to push to master, there is no merge conflict because User A has not touched file2.txt.

## Part 5:

When user A tries to git pull (before git push), they will encounter a merge conflict, since file1 has been changes by both users. To push, they must fix this merge conflict.
