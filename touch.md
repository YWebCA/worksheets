# Worksheet: `touch`

**Before you begin**, make sure your `~/temp/` directory exists and is empty.

Open iTerm and go home (if you're not there already).

## Do this in zsh:

    $ mkdir -p temp/kiwis
    $ cd temp/kiwis
    $ touch newfile.txt

What did that last line do?

> Hint: try `ls`.

> It created a new file called `newfile.txt`.

Try `touch`ing some more stuff. What is happening when you do that?

> It creates new files of whatever name (and type!) we tell it.

## Open one of your `touch`ed files in Sublime

Use the `subl` command and give it the name of your file as an argument.

What's in it?

> Nothing!

Can you `touch` files of different extensions? Try an HTML file. What happens
when you open it? What happens when you open it in Chrome? What happens when you
oen it in Sublime?

> Yes, we can touch files of any extension, even files with no extension. When
> you open one of these files, it's totally empty. HTML files opened in Chrome
> are blank. Files opened in Sublime are blank. `touch`ed images are empty, too.

-----

## Timestamps

Try

    $ ls -l

and find the timestamps for each file. What is a timestamp?

> The time we created the file.

Use `touch` on your oldest file and then `ls -l` again. What's changed?

> The timestamp updated to the current time.

**So what does `touch` *really* do?**

> Without changing a file, it updates the timestamp. If the file does not exist,
> it creates it.
