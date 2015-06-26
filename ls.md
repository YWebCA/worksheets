# ls

**Before you begin**, make sure you've done the `mkdir` worksheet and everything
worked properly. If you didn't set it up correctly, you're going to have some
trouble completing this worksheet.

`ls` is another abbreviation. Let's figure out what it does. Open iTerm and type

    $ cd temp
    $ ls

What output does the terminal give you?

<!-- Replace this comment with your answer -->

Try:

    $ cd stuff
    $ ls

Try:

    $ cd things
    $ ls

Try:

    $ cd frank
    $ ls

What do you think `ls` does? What does it stand for?

> `ls` is short for "list" and it lists the contents of the current working
> directory.

Try:

    $ cd joe
    $ ls
    $ cd alex
    $ ls
    $ cd john
    $ ls

What output do you get when you `ls` when you're in `~/stuff/things/frank/joe/alex/john`? Why?

> I get the contents of `john` which is nothing. The command was successful but
> nothing was output. This is because `john` is empty.

Try:

    $ cd ..
    $ ls
    $ cd ../../../
    $ ls
    $ cd ../../
    $ ls

How is `ls` different from `pwd`?

> `ls` shows you the contents of the current working directory, while `pwd`
> tells you the path to the current working directory.

## Notes on Flags

`-l` gives the long version of the list, complete with owner, files, permissions, etc.

`-a` shows *all* the files, including the hidden ones (that start with a
dot `.`).

I can combine these flags to do

    $ ls -al

or

    $ ls -la

and see all the hidden files in long format.
