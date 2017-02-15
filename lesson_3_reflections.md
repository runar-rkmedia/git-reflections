#### When would you want to use a remote repository rather than keeping all your work local?

I can easily share my code with others, collaborate and it serves as a backup to my local repository. I can even edit and add files from any computer

#### Why might you want to always pull changes manually rather than having Git automatically stay up-to-date with your remote repository?

Since commits are meant to be of just a single logical change, and often not a complete function for the end-user, pushing every commit wouldn't be meeningful as it would add code that might not be used, not tested, and even knowingly not working.

If the changes are big enought that one would want to share them, one can easily push.

#### Describe the differences between forks, clones, and branches. When would you use one instead of another?

##### Forks

Forks are a copy, or a clone, of a repository. I can fork somebody else's work if I want to have my own copy. I can change it however I want. The original is unaffected, but it does show all the forks that that repository has been the 'host' or 'origin' for. All forks will also link back to the original. This is to give credit to the original source.

After making some changes, I can still contribute to the original code from my fork.

#### Clones

Clones are copies of a repository, either from an online server, or a local one. It includes all history, remote-data and such, so one can easily clone and contribute.

#### Branches

Branches are a split of the code, where one might want to temporary go in different directioon, try out some new features or rewrites, without modifying the master-branch. One can create and switch branches easily, and later combine the brancshes when the time is right.

#### What is the benefit of having a copy of the last known state of the remote stored locally?

It means we know if the remote has changes, and we can update or continue working on this version. Merging can be done at a later time, but will sometimes cause mergeconflicts.

It also means that one can work offline with that version retrieved.
