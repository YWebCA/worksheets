# mkdir

You'll find that most of the command-line commands are going to be abbreviations
or acronyms because, guess what?, we're going to be typing them a lot and we'll
want them to be short.

Find out what `mkdir` stands for.

    Make Directory

What's a directory?

    A file that holds other file. A "folder", like in a filing cabinet.

## Commands and arguments

So far we've given naked commands such as `pwd` and `hostname`. When we use
those commands, we're actually invoking small progams. A program generally does
three things, and generally in this order:

1.  Take some information.
2.  Do some work.
3.  Give a result.

When the program makes changes to itself or its environment, that's called a
"side effect".

What makes commands interesting is that we can give them information to work
with, right on the command line. These pieces of information are called
"arguments". A command can be followed by one or more arguments. Arguments are
separated by spaces.

Open up iTerm and type

    $ cd ~

Then do this:

    $ mkdir temp
    $ mkdir temp/stuff
    $ mkdir temp/stuff/things
    $ mkdir temp/stuff/things/frank/joe/alex/john

What happened when you tried that last command? Why?

> I got an error!

    mkdir: temp/stuff/things/frank/joe/alex: No such file or directory

> You can't roof a house that doesn't have walls. Which is to say, you can't
> make directories inside directories that don't yet exist.

Try this:

    $ mkdir -p temp/stuff/things/frank/joe/alex/john

Let's look at what we did in the Finder:

    $ open .

What side effects do you see?

> All the directories were created leading up to john. `-p` stands for path and
> it patches all the holes in the path.

## Options

Sometimes arguments are options. Options come in two flavors: short:

    -v

and verbose:

    --verbose

Short options can be ganged up, like this:

    -aLm

Are options case-sensitive?

> Yes! `-r` is different from `-R`.

What does the `-p` option do when you invoke `mkdir` with it?

> It also creates the necessary intermediate directories that do not yet exist.
