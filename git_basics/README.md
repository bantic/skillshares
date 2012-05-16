Git Basics
==========

A basic overview of [Git](http://git-scm.com) accompanied by some tips,
tricks, and opinions on workflow for using it each day. This is no way
attempts to be a complete guide, just a simple set of heuristics to help
out beginners new to Git.

I personally learned Git best by watching Scott Chacon's
[videos](http://blip.tv/scott-chacon), reading through [Git's
documentation](http://git-scm.com/documentation), and browsing through
Chacon's [Pro Git book](http://git-scm.com/book). Remember, [Stack
Overflow](http://stackoverflow.com/tags/git/) is your friend, as well.


What is Git?
------------

This question has been covered numerous times all over the internet, but
I think of Git as a way of saving files at specific points in time. This
way, in case you mess anything up, you can go back to a specific point
and work from there.

Git also allows you to experiment freely with projects. If you had a car
project and wanted to add wings to it, you could do so by setting up a
`wings` branch. And, if anything went wrong, you could just rewind time
to a `commit` where the car previously worked perfectly.


Git Started
-----------

If you've never created a Git repository before, then let's start from
there on the command line.

First, we'll create a new project.

    $ mkdir letters
    $ cd letters

And we'll initialize this as a Git repository.

    $ git init

Now it's time to add some files. We'll do so using the `touch` command
and Unix bracket completion.

    $ touch README.md
    $ touch {a,b,c}.txt

You should now have four blank files in your repo. Let's go ahead and
create our first commit.

    $ git add --all
    $ git commit -m "First commit"