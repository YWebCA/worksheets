# Wildcard Matching

## Setup

    $ cd ~/temp
    $ touch ex12.txt ex13.txt ex14.txt ex21.txt
    $ touch ex12.html poet.html
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

<!-- Replace this comment with your notes -->

    $ ls ex*.*

What does `ls` output?

<!-- Replace this comment with your notes -->

    $ ls ex*

What does `ls` output?

<!-- Replace this comment with your notes -->

    $ ls *t

What does `ls` output?

<!-- Replace this comment with your notes -->

As you can see, `ls` takes an argument. We can tell it what (inside the current
working directory) to list. And by using wildcards, we can give it a formula for what to list.

## Wildcards and other commands

Other commands will take wildcards in their arguments. Try:

    $ cat *.txt > bigfile.txt

What is inside `bigfile.txt`?

<!-- Replace this comment with your answer -->

Remember back to pipes and redirects. Remember that `>` will overwrite any file you send output to. Why does `bigfile.txt` have all of the files in it and not just the last one?

<!-- Replace this comment with your answer -->

`rm` can take wildcards, too!

    $ rm *.txt
    $ ls

What happened?

<!-- Replace this comment with your answer -->
