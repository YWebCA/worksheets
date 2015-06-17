# `less`, `more`, and `cat`

## Prep

You can use the files you created in previous exercises for this worksheet.
If you're starting from scratch, you'll want something like this:

* Working directory: `~/temp/`
* Contents:
  	* `one.txt` &ndash; an empty file
  	* `two.txt` &ndash; a short file (5 lines or so)
  	* `three.txt` &ndash; a long file (about 100 lines)  

-----

## `less`

Try this...

    $ less

What happens?

<!-- Replace this comment with your answer -->

Unlike other commands, `less` doesn't return us to the command prompt
immediately. It keeps running and waits for us to give it instructions. Press
`q` to quit `less`. How did I know that `q` was quit? Let's try this:

    $ less --help

Read some of that output&mdash;enough that you understand what's going on. Now
you know how to *control* `less` once it's running. That's good. Because now you
can use all those controls just to navigate `less --help`!  

-----

### Verbose Options

`--help` is similar to options/switches/flags we've seen before, but it's the
**verbose** version of a flag. That means it starts with a double-dash (`--`)
and is one or more words connected by dashes. An example we've already used
is `--without-npm`.

Use `less --help` to find the short version of the `--help` flag and then test
it out.

<!-- Replace this comment with your notes -->

-----

### The Real Exercise

Finally, invoke `less` and give it one of your text files as an argument. Move
around a bit and then quit.

Try `less` with *two* arguments.

What happens? How do you change between files?

<!-- Replace this comment with your notes -->

-----

## `more`

In theory, `more` is a simpler version of `less` that can't go
backwards&mdash;it just exits when you get to the end of a file. It also has to
read an entire file before giving you control (which could be problematic for
very, very large files).

However, at least in Bash, `more` is just an alias for `less`, because `less` is
all  you need. Less is more. :) In Zsh, `more` works as expected.

<!-- Replace this comment with your notes -->

-----

## `cat`

1. Use `cat` on your empty file.
2. Use `cat` on your short file.
3. Use `cat` on you long file.
4. Give `cat` all your files at once.

What does `cat` do?

<!-- Replace this comment with your notes -->

What does `cat` *mean*? Which is to say: what is `cat` short for?

<!-- Replace this comment with your notes -->
