#### What happens when you initialize a repository? Why do you need to do it?

It makes **git** keep track of my files. I need it to make **git** track this project.

#### How is the staging area different from the working directory and the repository? What value do you think it offers?

It serves as a middlepoint. Say that I made some changes to multiple files, and then realized that the changes should be in multiple commits instead of just one. I can then stage just a few files, and then commit them. Next I'll add the other ones and commit them seperately in a tidy way.

This keeps my repository clean and tidy, so I can easily know which commit does what.

#### How can you use the staging area to make sure you have one commit per logical change?

We can use `git diff` without any arguments to see all differences between the last commit and files in the working directory. Use `git diff --staged` to see differences between last commit and the staging area.

By manually adding files to the staging area before a commit, we make sure that some thought goes into each commit. One can add only a single file, or many, depending on the change made.


#### What are some situations when branches would be helpful in keeping your history organized? How would branches help?

If one wants to do something experimental, while still having the regular working code available, branching is good. While working on a branch, one can easily switch to the master-branch if needed.

#### How do the diagrams help you visualize the branch structure?

One can see where each branch splits of from.

#### What is the result of merging two branches together? Why do we represent it in the diagram the way we do?

We combine the code from the two branches. **Git** tries its best to the this automaticly, by looking at the changes in the files, and their mutual ancestor. But sometimes merge conflicts happen. **Git** warns about this, and one can use `git mergetool` to help with this.

#### What are the pros and cons of **Git**’s automatic merging vs. always doing merges manually?

Pro: Combining merges manually would be a pain. Via a simple command, **git** can do this for us.

Con: Sometimes conflicts arises, and we need to go through them. **Git** however marks these conflicts for us, so it is much easier to deal with.
