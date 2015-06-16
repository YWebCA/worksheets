# mkdir

You'll find that most of the command-line commands are going to be abbreviations or acronyms because, guess what?, we're going to be typing them a lot and we'll want them to be short.

Find out what `mkdir` stands for.

<!-- Replace this comment with your answer -->

What's a directory?

<!-- Replace this comment with your answer -->

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

<!-- Replace this comment with your answer -->

Try this:

    $ mkdir -p temp/stuff/things/frank/joe/alex/john

Let's look at what we did in the Finder:

    $ open .

What side effects do you see?

<!-- Replace this comment with your answer -->

## Options

Sometimes arguments are options. Options come in two flavors: short:

    -v

and verbose:

    --verbose

Short options can be ganged up, like this:

    -aLm

Are options case-sensitive?

<!-- Replace this comment with your answer -->

What does the `-p` option do when you invoke `mkdir` with it?

<!-- Replace this comment with your answer -->
