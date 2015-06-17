# cd

`cd` stands for change directory, which is simply what it does. We use `cd` to move up and down the directory structure.

Enter the following commands to see `cd` at work:

    $ cd temp
    $ pwd

What did `pwd` return?

<!-- Replace this comment with your answer -->

Enter the following:

    $ cd stuff
    $ pwd

What did `pwd` return?

<!-- Replace this comment with your answer -->

What would happen if you entered `cd things`?

<!-- Replace this comment with your answer -->

Try it:

    $ cd things
    $ pwd

We can also optionally add a `/` to the end of the directory name. Other than being optional, `/` has a use we will go over in a bit.

Try adding a slash:

    $ cd frank/
    $ pwd

Try:

    $ cd joe/
    $ pwd

Try:

    $ cd alex/
    $ pwd

Try:

    $ cd john/
    $ pwd

You should now be at `/user/[your directroy]/temp/stuff/things/frank/joe/alex/john`. So how do we go back our previous directories. To go to a parent directory `cd` accepts `..` as a directory name. Any time you enter `cd ..` you will go to the parent directory of the one you are in. Try it out:

    $ cd ..
    $ cd ..
    $ pwd

What directory are in now?

<!-- Replace this comment with your answer -->

What directory would you be in if you did `cd ..` twice again?

<!-- Replace this comment with your answer -->

Try it again:

    $ cd ..
    $ cd ..
    $ pwd

You can also chain together directories and `..`s with `/` marks.
Try it:

    $ cd ../../..
    $ pwd

How many parent directories did you go up?

<!-- Replace this comment with your answer -->

What directory are you in?

<!-- Replace this comment with your answer -->

Try chaining together directories:

    $ cd temp/stuff/things/frank/joe/alex/john
    $ pwd

What directory are you in?

<!-- Replace this comment with your answer -->

How many child directories down did you go?

<!-- Replace this comment with your answer -->

And one last time:

    $ cd ../../../../../../../
    $ pwd

What directory are we finishing in?

<!-- Replace this comment with your answer -->

## Go home

By now you've seen this tild&egrav; `~` thing a few times. The tild&egrav; is
shorthand for your home directory. Since eveyone's home directory has a
different name, this is really useful, especially if you want to write code
other people can use.

When you open a terminal, you should automatically be at your home. You may have noticed, as you `cd` around, that your prompt changes to reflect your current
working directory. When you're home, your prompt shows a tild&egrav;.
Pretty cool.

Because we have this shorthand, getting home from anywhere is really easy:

    $ cd ~

Actually, you can just type

    $ cd

to go home. Programmers are lazy.

Since it's so useful to go home, we'll want to be able to easily find our home
directory in Finder and save it in our favorites for later.

    $ open ~/..

This opens the parent of our home directory in Finder. You should see a house
icon and the name of your home directory. If it's not already there, we're going
to click and drag that little house into our "favorites" menu on the left. Make
sure to drop it between items, not on or inside of anything.
