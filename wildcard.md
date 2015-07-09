# Wildcard Matching

## Setup

    $ cd ~/temp
    $ touch ex12.txt ex13.txt ex14.txt ex21.txt
    $ touch ex12.html poem.html
    $ mkdir heart
    $ mkdir egret

## Exercise

When you're playing a card game, sometimes there are wildcards. A wildcard can
be anything. When twos are wild, a two of diamonds can stand in for any other
card.

That's the idea behind wildcards here. On the command line, asterisks `*` are
wild. An asterisk can stand in for one or more characters. Just how you can use
wildcards to make a great poker hand, we can use asterisks to make more matches.

It's hard to explain, so let's try it:

    $ cd ~/temp
    $ ls *.txt

What does `ls` output?

> It shows only all the files with the `.txt` extension.

    $ ls ex*.*

What does `ls` output?

> All the files that start with `ex` and have a dot in the end.

    $ ls ex*

What does `ls` output?

> All the files that start with `ex`.

    $ ls *t

What does `ls` output?

> All the files that end with `t`. This includes directories. And because when you `ls` a directory, it shows its contents, we also get the contents of the directories that end in `t`.

As you can see, `ls` takes an argument. We can tell it what (inside the current
working directory) to list. And by using wildcards, we can give it a formula for what to list.

## Wildcards and other commands

Other commands will take wildcards in their arguments. Try:

    $ cat *.txt > poem.txt

What is inside `poem.txt`?

> The contents of all the files that match `*.txt` catted into `poem.txt`.

Remember back to pipes and redirects. Remember that `>` will overwrite any file you send output to. Why does `poem.txt` have all of the files in it and not just the last one?

> The `cat` command finishes and sends all of its output into `poem.txt` all at once.

`rm` can take wildcards, too!

    $ rm *.txt
    $ ls

What happened?

> All of the text files were removed! It didn't even bother to ask.
