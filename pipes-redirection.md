# Pipe and Redirect

Go to your home directory.

Redirects `<`, `>`, and `>>` are used input files to a command or put a commands output to a file.

## &gt;

`>` will send output of a command to a file. It will create the file if it doesn't exist and overwrite it if it does. Try:

    $ echo "Roses are red" > one.txt
    $ echo "Violets are blue" > one.txt
    $ cat one.txt

What's inside `one.txt`?

<!-- Replace this comment with your answer -->

    $ echo "Sugar is sweet\nAnd so are you" > two.txt

> Note the `\n`. Remember how backslashes can escape special characters? In this
> case, `\n` is a special code for a new-line character.

## Pipe

Pipe, `|`, is used to send the output of one command to another command. Let's
try concatenating some files and outputting them with less:

    $ cat one.txt two.txt | less

## &lt;

`<` will send a file's contents to a command. Try it out:

    $ cat < two.txt

Where does the output of the cat command come from?

<!-- Replace this comment with your answer -->

Try it with the less command:

    $ less < two.txt

Try using pipe and redirect together:

    $ less < two.txt | cat | less

What order do you think all these commands happened in?

<!-- Replace this comment with your answer -->

## &gt;&gt;

`>>` is used to *append* the output of a command to a file.

Let's try using it:

    $ echo "Roses are red" > three.txt
    $ cat three.txt >> poem.txt
    $ cat poem.txt
    $ cat one.txt >> poem.txt
    $ cat poem.txt
    $ cat two.txt >> poem.txt
    $ cat poem.txt

What happenned each time we entered used `>>`? What does "append" mean?

<!-- Replace this comment with your answer -->
