Git-Achievements records all of the achievements you acquire while using Git.

There are over 40 achievement, most with different levels to be achieved.
After a git command is executed if a new achievement is unlocked
git-achievements will display a message on the console for your enjoyment:

********************************************************************************
                            Git Achievement Unlocked!                            

                                    Caretaker                                    
                    Added a .gitignore file to a repository.                    
********************************************************************************


GitHub Pages
------------

A log of all of your achievements is kept locally, but you can also publish
it to GitHub pages so you can share your achievements (and there is a rss
feed so people can track your achievements).

For example here is the project maintainer's achievements page: http://icefox.github.com/git-achievements

If you are viewing a forked version of git-achievements you want to replace icefox/oppih
with the github user account you want to see like so:

    http://<username>.github.com/git-achievements

To push your achievements to GitHub first fork the project on GitHub,
clone *your* repository and set the following config to true:

    git config --global achievement.upload "true"

When an achievement is unlocked the index.html file will be overwritten,
committed and then a 'git push origin' will be executed.


Install
-------
1. fork this project to your GitHub account.
2. clone this repository to you machine. eg. clone to ~/.git-achievements
3. Add git-achievements to your path and alias git to git-achievements

>For example add the following to the end of your ~/.bash_profile

    export PATH=$PATH:$HOME/.git-achievements
    alias git="git-achievements"

You can get your first achievement by running

    git achievements --help


**Google Analytics**
-------
I added my Google analytics account ID. you can add yours in about line 450 or just remove these lines there.

Work on mutilple machines
-------
git-achievements will store your git action log in:
    $HOME/.git-achievements-action.log
    $HOME/git-achievements.log
So if you want to continue your git achievements on anather machine, you should manually cp these two file.
I have not file proper ways to keep the logs with git since everytime you use git(=git achievements),
  you will change the log file and it will require you to commit or stash...
  A loop, right?

So if you just want to use this 'git-achivements' as a tool to record your git commands achievements,
   you can add these two log file into your reprository.
   If you want to improve this project, you'd better comment out the alias line in your .bashrc :)
