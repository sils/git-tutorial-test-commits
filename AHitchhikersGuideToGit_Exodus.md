# Introduction

## What is This?

This post is the second of a series of three blog posts that tries to provide a **gentle introduction** to git. It follows the premise:

> If you know how a thing works, you can make it do what you want it to.

I'm assuming you either **read the first part** (TODO LINK), Genesis, or skipped it because you know all thats done in there.

## Overview

Here, again, the overview, we're doing the **second part** today.

### Genesis

**Genesis (i.e. "Creation" or "Beginning")**, covered some very basic things:

 * **Configuring** git so you can use it how you want. (Basic, aliases)
 * **Creating** your git **repository** (play god once!)
 * **Creating** your first git **commits**.
 * **Learning** what the **repository** is and **where commits get stored**.
 * **Browsing** through **history**.
 * **Ignoring files**.

### Exodus

This tutorial, **Exodus (i.e. "going out")** covers:

 * **Storing** temporary changes **without committing**.
 * **Navigating** commits in git.
 * **Sharing** commits to a **remote place**.
   * **Locally** (huh, that's sharing?)
   * Via **email**
   * To a **server**
   * To a **client**
 * Working **with others** (i.e. **non-linear**).
   * **Join** things.
   * **Linearize** things.
 * **Writing good** commits.
 * **Editing** commits. (Actually not editing but it feels like that.)

### Apocalypse

**Apocalypse (i.e. "uncovering")** will try to uncover some more advanced features of git, finally freeing your mind from your non-versioned filesystem:

 * **Finding more information** about code.
 * **Finding causes of bugs** in git.
 * **Reverting** commits.
 * **Reviewing** commits.
 * **Travelling though time** and **changing history** (you want me to believe you've never wanted to do that?)
 * **Getting back** lost things.
 * Let git **do things automatically**.

## Disclaimer

I wrote this tutorial to the best of my knowledge and experience, if you spot an error or find something important is missing, be sure to drop me a message!

## Preparation...

Don't forget your towel, whatever you do! If you still don't have one, go, get one! Now!

# Branching

## What Is a Branch?

You've waited long for this in the first tutorial, desperately - and I failed you. I'm sorry, wanted to cover the groundwork first. So let's get to this:

Do you recall that weird `HEAD` file in the `.git` directory I promised to explain a bit more last time? That `HEAD` file was a **pointer to the current commit** which contained the **files** we **compare our filesystem** with. Furthermore we saw that this `HEAD` file actually **didn't reference the commit directly**. It referenced some **master** file:

```
$ cat .git/HEAD 
ref: refs/heads/master
```

This file, `refs/heads/master`, contained just the **ID of the current commit**. This file **is** the **master branch**.

So to **summarize**: a **branch** is nothing more than a pointer (i.e. alias) to some commit.

## How Can We Use Branches?

Let's try out the `git branch` command:

```
$ git branch
* master
```

The branch command shows us what branches are available. Obviously there is this master branch there - which corresponds finely to the `refs/heads/master` file.

## TODO CHECKOUT

## Committing on a Branch

When **making a commit on a branch** the current branch gets **updated automatically**, i.e. it **points to the new commit**.

# TODO

Exodus (i.e. "going out") will cover:

    Store temporary changes without committing.
    Navigating commits in git.
    Sharing commits to a remote place.
        Locally (huh, that's sharing?)
        Via email
        To a server
        To a client
    Working with others (i.e. non-linear).
        Join things. git cat-file -p
        http://www.quora.com/How-does-Git-merge-work
        Linearize things.
    Writing good commits.
    Editing commits. (Actually not editing but it feels like that.)

