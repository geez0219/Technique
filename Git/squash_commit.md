## Squash commit 
To squash the commit from <start> to <end>

### Step 1.
``` git rebase -i <the_commit_one_before_start>

### Step 2
Git will automatically lead you to GNU nano page, you will see something like: <br>
pick 29d6a72 ... <br>
pick 590f0c3 ... <br>
...

Except for the first pick line, replaced all "pick" to "squash" and save it.

### Step 3
Git will automatically lead you to another GNU nano page, you can edit your commit message there. 

