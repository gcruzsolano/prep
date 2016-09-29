# Back Command Line Essentials

`bash` is the most powerful, prominent command line in history.
Every Mac and Linux machine comes with it and [Windows *finally*
added it](https://github.com/skilstak/faq/blob/gh-pages/microsoft.md)
to their developer version. This is the reason we have a `skilstak.sh`
is to ensure everyone learns the power of the command line as
professional do. At this point you should already known how to connect
with the [Terminal](terminal.md) or [CodeAnywhere](codeanywhere.md).

## Login

After you login you will see the *message of the day*, which includes
a reminder that you can type `h` to get the help from anywhere.

![](/assets/motd-h.png)

## Help

Nope, it is not `help`, (which is used for something else by the
system), it’s `h`.

![](/assets/h.png)

By the way, this is a little thing we added that is not normally there
for SkilStak™ students.

## List Files and Directories

You probably know what a file is. A ***directory*** is another name
for a folder and usually has a folder icon, but no icons on the
command line. Here’s how to list stuff. Notice that the files are
different colors. We will get to that in a minute.

![](/assets/ls.gif)

## Long Listing

If you add a `-l`, so `ls -l` (there’s a space there) it will show you
the same thing, but in a longer listing. From this long listing you
can see that the information about each thing is different. Again,
we’ll get into that more later. For now just know what one of the
files is a program that can be run and the other a plain text file.

![](/assets/ls-l.gif)

## Long Listing of a Single File

You can isolate the `ls` command to just show one or more things. This
time we just want to look at the `hello` program.

![](/assets/ls-l-hello.gif)

## Long Listing of Everything

Unix and Linux have a nice way of hiding stuff. This makes it less
cluttered. Sometimes, however, you want to look at it all. That’s what
the `-a` is for, so `ls -la`.

![](/assets/ls-la.gif)

## Clearing the Screen

At this point you screen is probably getting pretty cluttered up. The
`clear` command does just that so you can start fresh. Don’t worry,
everything is still there.

![](/assets/clear.gif)

## You are Here

The `pwd` command is for when you are wondering where you are. It
stands for “print working directory” but just know that it shows you
the ***full path*** to where you are in the file system.

![](/assets/pwd.gif)

## Make a Directory

Let’s make a directory to put our stuff in. In fact, let’s make the
special `repos` directory that we all use at SkilStak™ to store our
GitHub repos.

![](/assets/mkdir-cd-repos.gif)

Notice as soon as we make it we change directories into it. The
command is `cd repos` to do that.

## Change Up One Directory

To change to the directory one level above where we are, sometimes
called the *parent directory* use the special `..` directory:

![](/assets/cd-dotdot.gif)

## Change to the Home Directory

If you use `cd` without anything else it assumes you want to go back
to start, to your home directory.

![](/assets/cd.gif)

## Using Tab Completion

If you have played Minecraft at all they you have been well trained in
tab completion. It is when you type tab to get the computer to help
you out by guessing what the next thing to type is. In this example we
use it to type out the only directory names that are there. The screen
will blink when there are no more options when you keep hitting tab.
If there is more than one option pushing tab a second time lists out
all the possibilities that you can then use to continue typing the one
you want.

![](/assets/tab-completion.gif)

Understanding tab completion is the difference between a good command
line magician and a freaking 25th level wizard. Get used to using it.

## Change to User’s Home Directory

If you have permission and want to use a shortcut to go to another
user’s home directory put the user name after the tilde with no space.

![](/assets/cd-tilde.gif)

Notice we have set it up so you can’t peek at your neighbors by
default.

## Creating, Setting Permissions, and Editing a Script

There is a lot in this step but we put it all together because you are
going to be doing it a lot. 

First we create the file with the `touch hello` command, which just
makes an empty file if the file doesn’t exist. If it does, it updates
the time the file was last modified, which is its original purpose.

Next, we `chmod +x hello` to make the new file a runnable script.
Another term for this is *executable*. Hence the `x`.

Finally we open the file with the `vi` editor, (which is actually `vim`
but `vi` has been used for more than four decades).

![](/assets/touch-chmod-vi-hello.gif)

After we close the file we can now simply run it. We get into more
about what is in the file, including the shebang line, in the
[Fundamentals in Python](http://pyfun.skilstak.io) course.

## Renaming

For no particular reason let’s rename the file.

![](/assets/mv-hello-hi.gif)

## Copying

How about a copy?

![](/assets/cp-hi-nyan.gif)

## Removing File

Now we can remove our `hi`.

![](/assets/rm-hi.gif)

## Removing Directory 

Now we can create a directory to put it in, only to delete it.

![](/assets/rm-rf-foo.gif)

***Use this command with extreme caution. Even though we use GitHub to
backup everything this `rm -rf dir` command will not ask. It will
completely destroy the `dir`. If you mistakenly write the wrong `dir`
or dots or worse you will irrecoverably destroy it. There is no
undo! This is why they call it a command line.***

## Editing Existing File

Just point `vi` at the file. 

![](/assets/vi-hello.gif)

Here are the essentials for navigating around and doing things in
`vi`. It takes a bit longer to learn than other editors but the
rewards are well worth it. `vi` is both the most powerful and most
prominent editor ever created. It is literally on every single
Linux/Mac/Unix machine in the world and has been for more than four
decades. **No other editor can make that claim, period.**

![](/assets/vim-essentials.png)

## Save to GitHub

This is all you need to `save` your work for now. This is actually
several `git` commands combined to make it easier to start out.

![](/assets/save.gif)

## Stop the Fish

And before we go. Type `ctrl-c` to stop pretty much *anything*
running on the command line, (although `vi` must be exited properly).
Start the fishes with `fish` and stop them with `ctrl-c`.

![](/assets/fish-ctrl-c.gif)

## Just a Start

This is just the tip of the iceberg. Learning command line will help
you dominate technology and harness its power for you to make amazing
things.

---
[![home](/assets/home-bw.png)](/README.md)
[![cc-by-sa](/assets/cc-by-sa.png)][cc-by-sa]
[![skilstak](/assets/skilstak-logo-bw.png)][skilstak]
[cc-by-sa]: https://creativecommons.org/licenses/by-sa/4.0/
[skilstak]: http://skilstak.io

