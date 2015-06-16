# `less`, `more`, and `cat`

[Right-click and "Save link as..." to download this worksheet.](worksheets/less-and-more.md)

## Prep

You can use the files you created in previous exercises for this worksheet. If you're starting from scratch, you'll want something like this:

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

So try this...

	$ less --help

Read some of that. Now you know how to *control* `less` once it's running. That's good. Because now you can use all those controls to navigate `less --help`!  

-----

### Verbose Options

`--help` is similar to options/switches/flags we've seen before, but it's the **verbose** version of a flag. Use `less --help` to find the short version and then test it out.

*Additional notes:*  

-----

### The Real Exercise

Finally, use `less` and give it one of your text files as an argument. Move around a bit and then quit.

Try `less` with *two* arguments.

What happens? How do you change between files?

*Additional notes:*  

-----

## `more`

In theory, `more` is a simpler version of `less` that can't go backwards. However, at least in Bash, `more` is just an alias for `less`, because `less` is all  you need.

Do let me know if I'm wrong about that. I love being wrong because then I get to be right for certain. :)

*Additional notes:*  

-----

## `cat`

1. Use `cat` on your empty file.
2. Use `cat` on your short file.
3. Use `cat` on you long file.
4. Give `cat` all your files at once.

What does `cat` do?

What does `cat` *mean*? Which is to say: what is `cat` short for?

*Additional notes*:  
