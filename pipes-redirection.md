# Pipe and Redirect

Go to your home directory.

Redirects `<`, `>`, and `>>` are used input files to a command or put a commands output to a file.

## &gt;

`>` will send output of a command to a file. It will create the file if it doesn't exist and overwrite it if it does. Try:

    $ echo "Roses are red" > ex12.txt
    $ echo "Violets are blue" > ex12.txt
    $ cat ex12.txt

What's inside `ex12.txt`?

<!-- Replace this comment with your answer -->

    $ echo "Sugar is sweet\nAnd so are you" > ex13.txt

> Note the `\n`. Remember how backslashes can escape special characters? In this
> case, `\n` is a special code for a new-line character.

## Pipe

Pipe, `|`, is used to send the output of one command to another command. Let's
try concatenating some files and outputting them with less:

    $ cat ex12.txt ex13.txt | less

## &lt;

`<` will send a file's contents to a command. Try it out:

    $ cat < ex13.txt

Where does the output of the cat command come from?

<!-- Replace this comment with your answer -->

Try it with the less command:

    $ less < ex13.txt

Try using pipe and redirect together:

    $ less < ex13.txt | cat | less

What order do you think all these commands happened in?

<!-- Replace this comment with your answer -->

## &gt;&gt;

`>>` is used to *append* the output of a command to a file.

Let's try using it:

    $ echo "Roses are red" > ex14.txt
    $ cat ex14.txt >> poem.txt
    $ cat poem.txt
    $ cat ex12.txt >> poem.txt
    $ cat poem.txt
    $ cat ex13.txt >> poem.txt
    $ cat poem.txt

What happenned each time we entered used `>>`? What does "append" mean?

<!-- Replace this comment with your answer -->
