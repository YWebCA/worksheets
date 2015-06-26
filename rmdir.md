# rmdir

> **Before you begin**, make sure you did the `mkdir` worksheet and everything
> worked properly. If you skipped it or there were errors, you're going to have
> problems here.

If `mkdir` is "make directory," take a guess: what does `rmdir` do?

> Remove a directory.

First, go to your home directory. Then change your working directory to `temp`
and list the contents:

    $ cd ~
    $ cd temp
    $ ls

Let's dive all the way into the `stuff` directory:

    $ cd stuff/things/frank/joe/alex/john/

Make sure `john` is empty by doing

    $ ls

and make sure you get nothing for output. Then we'll `cd` up one directory and
see what we have:

    $ cd ..
    $ pwd
    $ ls

Now try:

    $ rmdir john

What happened? (Hint: `ls` again to see the side effects.)

> The directory `john` was removed. **FOREVEEEEERRRRRR.**

Let's keep going:

    $ cd ..
    $ rmdir alex
    $ cd ..
    $ ls
    $ rmdir joe
    $ cd ..
    $ ls
    $ rmdir frank
    $ cd ..
    $ ls
    $ rmdir things
    $ cd ..
    $ ls
    $ rmdir stuff
    $ pwd
    $ ls

What did you just do?

> I backtracked up the directory tree, removing all the directories on the way.

## Try this on your own...

What happens if you try to remove a directory and it's not empty? Inside `temp`,
create the directories `a/` and `a/b/`. Try to remove `a/`. What happens?

> I get an error

    rmdir: a: Directory not empty

Let's clean up after ourselves:

    $ cd a
    $ rmdir b
    $ cd ..
    $ rmdir a

## Notes on Flags

I can ue the `-p` option to remove all the empty directories in a path, starting
with the childmost child. `-p` stands for "path".
