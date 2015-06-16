# Worksheet: `touch`

[Right-click and "Save link as..." to download this worksheet.](worksheets/touch.md)

More command line!

So we don't get super confused, let's delete the `temp` directory from our home folders. You can do this in the Finder.

Open Bash and go home.

## Do this in Bash:

    $ mkdir -p temp/kiwis
    $ cd temp/kiwis
    $ touch newfile.txt

What did that last line do?

> Hint: try `ls`.

Try `touch`ing some more stuff. What is happening when you do that?

*Additional notes:*  

## Open one of your `touch`ed files in Sublime

What's in it?

Can you `touch` files of different extensions? Try an HTML file. What happens when you open it? In Chrome? In Sublime?

*Additional notes:*  

-----

## Timestamps

Try `ls -l` and find the timestamps for each file. What is a timestamp?

Use `touch` on your oldest file and then `ls -l` again. What's changed?

**So what does `touch` *really* do?**

*Additional notes:*  

-----

## Experiment time

`cd` up one directory and try to `rmdir kiwis`. You *should* get an error. What is it and why do you get it?
