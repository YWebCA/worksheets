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

<!-- Replace this comment with your answer -->

`rm` will also take multiple arguments. Try the following command:
    
    $ rm iamcool.txt neat.txt thefourthfile.txt
    $ ls

What's left?

<!-- Replace this comment with your answer -->

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

<!-- Replace this comment with your answer -->

What does the `-f` flag mean?

<!-- Replace this comment with your answer -->

`rm -rf` seems like a quick and powerful command. Can you think of any reasons
why you might avoid using it?

<!-- Replace this comment with your answer -->

If `-f` is quick and risky, find a flag that helps us to be more careful.

<!-- Replace this comment with your answer -->
