# Pipe and Redirect

Pipe, `|`, is used to send the output of one command to another command. Let's try concatenating some files and outputting them with less:

    $ cat ex12.txt ex13.txt | less

Redirects `<`, `>`, and `>>` are used input files to a command or put a commands output to a file.

`<` will send a files contents to a command. Try it out:

    $ cat < ex13.txt

Where do the output of the cat command come from?

<!-- Replace this comment with your answer -->

Try it with the less command:

    $ less < ex12.txt

Try using pipe and redirect together:

    $ less < ex12.txt | cat | less

What order do you think the instances less and cat happened in?

<!-- Replace this comment with your answer -->

Try out the following command:

    $ cat ex13.txt > ex15.txt
    $ cat ex15.txt

Where did the contents of `ext15.txt` come from?

<!-- Replace this comment with your answer -->

`>>` is used to append the output of a command to a file. Let's try using it:

    $ cat ex13.txt >> ex15.txt
    $ cat ex15.txt
    $ cat ex13.txt >> ex15.txt
    $ cat ex15.txt

What happenned each time we entered `cat ex13.txt >> ex15.txt`?

<!-- Replace this comment with your answer -->