# Worksheet: `cp`

`cp` is an abbreviation for "copy." It can copy both files and directories.

## Refresh

Let's start with a fresh directory to play with. Open Finder and go to your home directory *or* type this in iTerm:

		$ open ~

Drag the `temp` folder to the **trash**.

Now in iTerm:

		$ cd ~
		$ mkdir -p temp/mangoes
		$ cd temp/mangoes
		$ touch one.txt

## Let's learn `cp`

		$ cp one.txt two.txt

What happened?

<!-- Replace this comment with your answer -->

Open `two.txt` in Sublime:

		$ subl two.txt

Type some stuff, save it, and close it. Now, in iTerm...

		$ cp two.txt three.txt

Open `three.txt` in Sublime. What's going on when you `cp`?

<!-- Replace this comment with your answer -->

Type some more stuff, save, and close `three.txt`. Now open `two.txt` in Sublime. What do
you see?

<!-- Replace this comment with your answer -->

What's in `one.txt`?

<!-- Replace this comment with your answer -->

### Be careful...

Try this...

	$ cp three.txt one.txt

What happened? Use Sublime to investigate.

<!-- Replace this comment with your answer -->

-----

## The `-r` switch

Now you're going to do some work on your own.

1.  Make at least two directories.
2.  Make two directories in each of the ones you just made.
3.  Create some empty files in each of the child directories.

Just as an example, this is what I have (but you can do whatever you like):

	katamari:temp LipGlossary$ ls -R
	fruit	veg

	./fruit:
	kiwis	mangoes

	./fruit/kiwis:
	brown.txt	green.txt

	./fruit/mangoes:
	ripe.txt	sweet.txt

	./veg:
	carrots	peppers

	./veg/carrots:
	orange.txt	purple.txt

	./veg/peppers:
	bell.txt	red.txt

Try moving around and using `cp -r` on different things, files *and*
directories. Remember that `cp` takes two arguments: a *source* and a
*destination*.

Describe what the `-r` switch does:

<!-- Replace this comment with your answer -->

-----

## Let's Play

Please ask the instructor how much of this section to complete. There are 56
cases, and you probably don't want to do them all by yourself.

Try all of these things:

1.  `$ cp source destination`
2.  `$ cp source/ destination`
3.  `$ cp source destination/`
4.  `$ cp source/ destination/`
5.  `$ cp -r source destination`
6.  `$ cp -r source/ destination`
7.  `$ cp -r source destination/`
8.  `$ cp -r source/ destination/`

for each of these cases:

1.  `source` does not exist
2.  `source` is a file and
		1.  `destination` is a file
		2.  `destination` is a directory
		3.  `destination` does not exist
3.  `source` is a directory and
		1.  `destination` is a file
		2.  `destination` is a directory
		3.  `destination` does not exist

### My Answers

<!-- Replace this comment with your answers -->

### Our Answers

1.  `source` does not exist
		1.  `$ cp source destination`
		2.  `$ cp source/ destination`
		3.  `$ cp source destination/`
		4.  `$ cp source/ destination/`
		5.  `$ cp -r source destination`
		6.  `$ cp -r source/ destination`
		7.  `$ cp -r source destination/`
		8.  `$ cp -r source/ destination/`
2.  `source` is a file and
		1.  `destination` is a file
					1.  `$ cp source destination`
					2.  `$ cp source/ destination`
					3.  `$ cp source destination/`
					4.  `$ cp source/ destination/`
					5.  `$ cp -r source destination`
					6.  `$ cp -r source/ destination`
					7.  `$ cp -r source destination/`
					8.  `$ cp -r source/ destination/`
		2.  `destination` is a directory
				1.  `$ cp source destination`
				2.  `$ cp source/ destination`
				3.  `$ cp source destination/`
				4.  `$ cp source/ destination/`
				5.  `$ cp -r source destination`
				6.  `$ cp -r source/ destination`
				7.  `$ cp -r source destination/`
				8.  `$ cp -r source/ destination/`
		3.  `destination` does not exist
				1.  `$ cp source destination`
				2.  `$ cp source/ destination`
				3.  `$ cp source destination/`
				4.  `$ cp source/ destination/`
				5.  `$ cp -r source destination`
				6.  `$ cp -r source/ destination`
				7.  `$ cp -r source destination/`
				8.  `$ cp -r source/ destination/`
3.  `source` is a directory and
		1.  `destination` is a file
				1.  `$ cp source destination`
				2.  `$ cp source/ destination`
				3.  `$ cp source destination/`
				4.  `$ cp source/ destination/`
				5.  `$ cp -r source destination`
				6.  `$ cp -r source/ destination`
				7.  `$ cp -r source destination/`
				8.  `$ cp -r source/ destination/`
		2.  `destination` is a directory
				1.  `$ cp source destination`
				2.  `$ cp source/ destination`
				3.  `$ cp source destination/`
				4.  `$ cp source/ destination/`
				5.  `$ cp -r source destination`
				6.  `$ cp -r source/ destination`
				7.  `$ cp -r source destination/`
				8.  `$ cp -r source/ destination/`
		3.  `destination` does not exist
				1.  `$ cp source destination`
				2.  `$ cp source/ destination`
				3.  `$ cp source destination/`
				4.  `$ cp source/ destination/`
				5.  `$ cp -r source destination`
				6.  `$ cp -r source/ destination`
				7.  `$ cp -r source destination/`
				8.  `$ cp -r source/ destination/`

-----

## The Big Takeaway

So now you know how to copy things into other things. But there are some weird
edge cases that you may have discovered above.

1.  How can you make sure you're copying a file into a subdirectory and not just
    copying into the working directory with a new name?

<!-- Replace this comment with your answer -->

2.  Did you figure out how to merge directories?

<!-- Replace this comment with your answer -->
