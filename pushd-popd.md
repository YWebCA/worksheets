# Worksheet: `pushd` and `popd`

[Right-click "Save link as..." to download this worksheet.](worksheets/pushd-popd.md)

This worksheet corresponds to [this chapter](http://cli.learncodethehardway.org/book/ex8.html) of the [Command Line Crash Course](http://cli.learncodethehardway.org/book/).

## Thinking with stacks

Before we jump into command line stuff, we have to talk about stacks.

A **stack** is a computer science concept. It is a data structure that you can imagine as a *stack* of paper on a table. You add new things to the top of the stack, one by one, and you remove things from the top of the stack, one by one.

When you add things to the stack, it's called "pushing," and when you remove things, it's called "popping."

Because we only manipulate the stack from the top, it's called a last-in-first-out (LIFO) data structure.

-----

### Exercise 1: consider the following series of events.

#### I have a stack that looks like this:

     baz     <- top
     bar
     foo
    -----    <- bottom

#### Now I do the following things:

1. push bat
2. pop
3. push zim
4. pop
5. pop
6. push grr
7. push dib
8. push gaz
9. pop

#### What does the stack look like now?  

*Additional notes:*

-----

### Exercise 2: use the original stack from Exercise 1.

#### Pop three times. What does the stack look like now?

*Additional notes:*

#### Pop again. What happens?

*Additional notes:*

-----

## Apply this knowledge to `pushd` and `popd`

Let's switch gears. Above, we were talking about stacks and stack operations (push and pop) in general. As you migh imagine, the Bash commands `pushd` and `popd` use a stack in order to work.

If the command `pwd` means "print working directory," what does `pushd` mean? What does `popd` mean?

### In 10 words or less, what does `pushd` do?

### Does `pushd` take an argument?

#### If so...

What is it (give an example) and what does it do?

*Additional notes:*

##### Is it optional?

If so, what happens if you don't give an argument?

*Additional notes:*

#### If not, why not?

*Additional notes:*

-----

### In 10 words or less, what does `popd` do?

### Does `popd` take an argument?

#### If so...

What is it (give an example) and what does it do?

*Additional notes:*

#### If not, why not?

*Additional notes:*

-----

### Explain the output `pushd` and `popd` give back to you

*Additional notes:*

### Do pushd and popd take any options?

*Additional notes:*