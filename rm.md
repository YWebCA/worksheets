# rm

Like `rmdir` is for removing directories, `rm` is for removing files. It's short
for "remove."

## Prep

Go to your temp directory and touch some stuff:
    
    $ cd ~/temp
    $ touch uncool.txt iamcool.txt neat.txt thefourthfile.txt
    $ mkdir something
    $ touch something/awesome.txt

Hopefully that's starting to feel comfortable.

## Exercise

When `rm` removes files, it *does not* send them to the trash. Those files are
**gone forever**. So use some caution here and make sure you know your working
directory and what you're typing.

Try this:

    $ rm uncool.txt

and look at the contents of the working directory:
    
    $ ls

Try the following commands:
    
    $ rm uncool.txt
    $ ls

What changed?

> We removed `uncool.txt`. When we tried to remove it again, we got an error, because it was already gone.

`rm` will also take multiple arguments. Try the following command:
    
    $ rm iamcool.txt neat.txt thefourthfile.txt
    $ ls

What's left?

> Only the `something` directory is left.

Copy your `something` directory to a `newplace` directroy:

    $ cp -r something newplace
    $ ls

Remove your `something` directory:

    $ rm something/awesome.txt
    $ rmdir something
    $ ls

## Options

We can use `rm` to remove directories along with their contents using the `-r`
flag:
    
    $ rm -rf newplace
    $ ls

We've seen the `-r` flag before. What other command takes `-r`? Does it mean the
same thing for both commands?

> `mv` and `cp` take the `-r` flag. It does mean the same thing: recursive (i.e. all the way down).

What does the `-f` flag mean?

> `-f` probably stands for "force". It suppresses errors and doesn't prompt for confirmation.

`rm -rf` seems like a quick and powerful command. Can you think of any reasons
why you might avoid using it?

> You could end up deleting a whole bunch of things you didn't mean to, especially when you forget what your working directory is.

If `-f` is quick and risky, find a flag that helps us to be more careful.

> The `-i` flag prompts you for everything you remove (unless overridden by `-f`).
