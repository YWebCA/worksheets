`cd` stands for change directory, which is simple what it does. We use `cd` to move up and down the directory structure.
Enter the following commands to see `cd` at work:
    $ cd temp
    $ pwd

What did `pwd` return?



Enter the following:
    $ cd stuff
    $ pwd

What did `pwd` return?



What would happen if you entered `cd things`?


Try it:
    $ cd things
    $ pwd

Try:
    $ cd frank/
    $ pwd

Try:
    $ cd joe/
    $ pwd

Try:
    $ cd alex/
    $ pwd

    $ cd john/
    $ pwd

You should now be at `/user/[your directroy]/temp/stuff/things/frank/joe/alex/john`. So how do we go back our previous directories. To go to a parent directory `cd` accepts `..` as a directory name. Any time you enter `cd ..` you will go to the parent directory of the one you are in. Try it out:
    $ cd ..
    $ cd ..
    $ pwd

What directory are in now?



What directory would you be in if you did `cd ..` twice again?



Try it again:
    $ cd ..
    $ cd ..
    $ pwd

You can also chain together directories and `..`s with `/` marks.
Try it:
    $ cd ../../..
    $ pwd

How many parent directories up did you go you?



What directory are you in?



Try chaining together directories:
    $ cd temp/stuff/things/frank/joe/alex/john
    $ pwd

What directory are you in?



How many child directories down did you go?



And one last time:
    $ cd ../../../../../../../
    $ pwd

What directory are we finishing in?


