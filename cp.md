# Worksheet: `cp`

[Right-click and "Save link as..." to download this worksheet.](worksheets/cp.md)

Let's nuke `~/temp` again. Then open Bash, go home, and...

	$ mkdir -p temp/mangoes
	$ cd temp/mangoes
	$ touch one.txt

## Let's learn `cp`

	$ cp one.txt two.txt

What happened?

Open `two.txt` in Sublime, type some stuff, save it, and close it. Now, in Bash...

	$ cp two.txt three.txt

Open `three.txt` in Sublime. What's going on? Type some more stuff, save, and close it. Now open `two.txt` in Sublime. What do you see? What's in `one.txt`?

*Additional notes:*  

### Be careful...

Try this...

	$ cp three.txt one.txt

What happened?

*Additional notes:*  

-----

## The `-r` switch

Make at least two directories. Put two directories in each of those. Now create some empty files in each of the "leaf" directories.

This is what I have (but you can do whatever you like):

	katamari:temp LipGlossary$ ls -R
	fruit	veg

	./fruit:
	kiwis	mangoes

	./fruit/kiwis:
	brown.txt	green.txt

	./fruit/mangoes:
	ripe.txt	young.txt

	./veg:
	carrots	peppers

	./veg/carrots:
	orange.txt	purple.txt

	./veg/peppers:
	bell.txt	red.txt

Try moving around and using `cp -r` on different things, files *and* directories. It takes two arguments, a *source* and a *destination*.

Describe what the `-r` switch does:

-----

## Let's Play

Set up each of these cases...

1. `source` does not exist?
2. `source` is a file and
	1. `destination` is a file?
	2. `destination` is a directory?
	3. `destination` does not exist?
3. `source` is a directory and
	1. `destination` is a file?
	2. `destination` is a directory?
	3. `destination` does not exist?

And, for each of them, try all of these things:

1. `$ cp source destination`
2. `$ cp source/ destination`
3. `$ cp source destination/`
4. `$ cp source/ destination/`
5. `$ cp -r source destination`
6. `$ cp -r source/ destination`
7. `$ cp -r source destination/`
8. `$ cp -r source/ destination/`

### My Answers

-----

## The Big Takeaway

So now you know how to copy things into other things. But there are some weird edge cases that you may have discovered above.

1. What's the subtle difference between copying a file to the working directory with a new name versus copying it into a directory while keeping its name?

2. Did you figure out how to merge directories?

*Additional notes:*
