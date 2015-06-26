# Worksheet: Markdown

**Markdown** is a markup language (confusing, I know) meant to make formatting
text super easy to read, easy to write, and easy to share.

When you write with a word processor and format your text, under the hood code
is being generated that will render the text into the formatting you see on the
screen. Problems occur when you want to convert text formatted in one program
into another program because they use different formatting languages! Markup
languages are special because they are formatting codes written by a human, not
a word processor. While this may sound like more work for you, it's actually
less work in the long run, because

1.  You have complete control over what's going on "under the hood."
2.  The same markup language can be rendered by many different compilers.
3.  One markup language can (usually) be transpiled into a different one.
4.  In transfering marked-up text to another program, system, or person,
    everything will remain identical and your formatting will stay intact.

So you actually get to save time reformatting things, and you can be sure that
what you see is what other people see.

Markdown does its best to make writing markup in your text simple and easy. It's
other goal is to make your markup easy to read, even before it's been rendered.
If you're reading this document in Sublime Text, it should look pretty
understandable. That's because it's written in Markdown!

Did you know?: most wikis use markup instead of rich text editing. If you've
ever edited Wikipedia, you've already encountered a different kind of markup
specific to the MediaWiki software. GitHub's wikis use Markdwon, and if you
write a README in Markdown, it will automatically render on your repository's
home page.

So lets learn Markdown!

## Install a Markdown previewer package for Sublime

Skip this section if you've already installed Markdown Preview.

Before you begin, make sure you have the [Package Control package installed in Sublime](sublime-text-2-package-control).

### Open the Sublime Command Palette

Use `⌘⇧P` (`COMMAND-SHIFT-P`) to bring up the Command Palette.

<!-- Add any additional notes here. -->

### Install a new package

Search for the Package Control command to install a new package.

<!-- Add any additional notes here. -->

### Install a Markdown previewer

Search for a Markdown Previewer package and install it.

<!-- Add any additional notes here. -->

## Preview this worksheet in the browser

Use Markdown Previewer to render this worksheet (the one you're looking at right now) in the browser. You're on your own for this one. How do you do it?

> Opened the command palette (Command+Shift+P) and searched for "Markdown" and selected "Preview".

Once you figure this out, it will be very easy to test your answers on the rest
of the worksheet.

<!-- Add any additional notes here. -->

## Learn how to use Markdown

As a developer, you're going to spend a lot of time searching the Internet for
pieces of knowledge to add to your mental toolbox. (That may not sound like fun,
but it sure beats going to the library or calling a professor!) Let's get used
to doing our own research right now. Open up Chrome and try to find some
resources to teach yourself Markdown.

Don't know where to start? Daring Fireball is the guy who's most "in charge" of
Markdown's development and maintenance. Use Google to find some of his
documentation.

### Figure out how to do all these block-level things in Markdown.

1.  A paragraph:

    > Just type! It's that easy. Have blank lines around the paragraph. Example:

    This is an example paragraph. Check it out!
    This line is not blank!

2. A heading (both ways):

    > Method 1: Underline the heading with equals (====) signs or dashes (-----)

        My Heading
        ==========

        My Subheading
        -------------

    > Method 2: Use a hash (#) at the beginning of the line.

        # My H1
        ## My H2
        ## My H3
        etc.

3.  An unordered list:

    > Begin the lines with plus signs `+`, asterisks `*`, or dashes `-`. You **may** be able to mix and match them. But you can definitely use them all separately.

        * Item 1
        * Item 2
        * Item 3

        + Thing 1
        + Thing 2
        + Thing 3

        - Stuff 1
        - Stuff 2
        - Stuff 3

        * This
        - That
        + The other

4. An ordered list:

    > Write a numbered list. The numbers don't have to be in order.

    2.  Hey
    1.  This
    1.  Is still valid

5.  A multiple-line list item:

    > Keep the following blocks also indented at the same level. An example:

    This is an example of a multi-line list item.

6.  A code block showing off some code that you don't want to render in the page:

    > Indent the code block one level deeper than your working indentation level.

        This is a code block!

7. A nested blockquote:

    > If a block quote uses one greater-than sign or closing angle bracket, then a nested block quote uses two.
    > > This is an example.
        
        > One block quote
        > > Nested block quote

8.  A horizontal rule:

    > A line consisting of three to five dashes or asterisks.
    >
    > > Three dashes gives a short anchor.
    > > `---`
    >
    > > Five dashes gives a thin line.
    > > `-----`
    >
    > > Asterisks give a thick line.
    > > `***`
    > > `*****`

What does "block-level" mean?

> In terms of a webpage, a block is an element that takes up the full width of its parent. It can contain other blocks. It can have sibling blocks.


### Figure out how to do all these inline things in Markdown.

1.  A link...  

    1.  "Automatically," such as an e-mail address:

        > Just type the email address. Example:

        annalise@adorable.io

        http://www.google.com

        www.google.com

        http://google.com

        > These don't work:

        google.com

        mail.google.com

        google.com/mail

    2.  With link text:

        Example: [Link text here](http://www.example.com)

            [Link text here](http://www.example.com)

    3.  A reference-style link in a paragraph:

            [Link text][id]

        > Then, later on in the document, you have to define the identifier.

            [id]: http://example.com/  "Optional Title Here"

        [Link text][id]

        Note: the definition cannot be indented at all.

        Why are reference-style links awesome?

        1.  You can put the definition anywhere in the document.
        2.  You can use the definitions more than once.
        3.  Your inline links are short and sweet.

2. Emphasis (two ways):

    > Emphasis is usually rendered italic. Surround some text with asterisks `*` or underscores `_`.

        _This is italic!_
        *So is this!*

    _This is italic!_

    *So is this!*

3. Strong emphasis (two ways):

    > Strong emphasis usually renders as bold. Surround some text with two asterisks or underscores.

        __This is bold!__
        **So is this!**

    __This is bold!__

    **So is this!**

3.  A literal asterisk or underscore:

    > Give your asterisks or underscores some breathing room with spaces. If they have to be next to other characters, escape them with a backslash `\`. Some examples:

        I'm typing along and I want to talk about
        \*\* asterisks! In multiple places! \*\*
        \_cool_username_dude_thing\_
        I have one \*asterisk here\* and there * .

4.  Inline code:

    `This` is an `example` of using `inline code segments`! 'Apostrophes' do not work.

        `This` is an `example` of using `inline code segments`! 'Apostrophes' do not work.

    Literal \` backtick \` or grave \`.

        Literal \` backtick \` or grave \`.

5. An image...

    1. Inline...  

        1.  Without alt text.

            ![](http://vignette2.wikia.nocookie.net/steven-universe/images/7/7b/TFW.png/revision/latest?cb=20140629185937)

        2.  With alt text.

            ![Tiny floating whaaaaaale!](http://vignette2.wikia.nocookie.net/steven-universe/images/7/7b/TFW.png/revision/latest?cb=20140629185937)

    2. Reference-style...  

        1.  Without alt text.

            ![][whale]  

        2.  With alt text.

            ![Tiny floating whaaaaale!][whale]

What does "inline" mean?

> Inline elements do not need their own blocks. They can flow in the same line as text. They are also called "span elements".

### Comments

You may have noticed "comments" scattered throughout this document. What is a
comment?

> A comment is not rendered in the final product.

    A comment starts with this: <!--

    A comment ends with this: -->

Why are they useful?

1.  I can write whatever I want, it doesn't have to be syntactically correct.
2.  I can use comments to remove parts of my code that are currently broken without deleting it.
3.  I can leave notes to myself.
4.  I can leave notes to my teammates.
5.  I can document code that's confusing.

What are some circumstances where you'd use comments?

> They're useful! See above.

### Can you mix and match Markdown markup and HTML markup?

If so, give an example. If not, why not? (If you don't know anything about HTML,
that's okay. Just do your best to answer.)

<!-- Replace this comment with your answer. -->

[id]: http://example.com/  "Optional Title Here"
[whale]: http://vignette2.wikia.nocookie.net/steven-universe/images/7/7b/TFW.png/revision/latest?cb=20140629185937 "Best cartoon ever!"