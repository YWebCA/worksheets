# Worksheet: `touch`

**Before you begin**, make sure your `~/temp/` directory exists and is empty.

Open iTerm and go home (if you're not there already).

## Do this in zsh:

    $ mkdir -p temp/kiwis
    $ cd temp/kiwis
    $ touch newfile.txt

What did that last line do?

> Hint: try `ls`.

<!-- Replace this comment with your answer -->

Try `touch`ing some more stuff. What is happening when you do that?

<!-- Replace this comment with your answer -->

## Open one of your `touch`ed files in Sublime

Use the `subl` command and give it the name of your file as an argument.

What's in it?

<!-- Replace this comment with your answer -->

Can you `touch` files of different extensions? Try an HTML file. What happens
when you open it? What happens when you open it in Chrome? What happens when you
oen it in Sublime?

<!-- Replace this comment with your answer -->

-----

## Timestamps

Try

    $ ls -l

and find the timestamps for each file. What is a timestamp?

<!-- Replace this comment with your answer -->

Use `touch` on your oldest file and then `ls -l` again. What's changed?

<!-- Replace this comment with your answer -->

**So what does `touch` *really* do?**

<!-- Replace this comment with your answer -->
