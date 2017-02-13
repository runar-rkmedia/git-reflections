#### How did viewing a diff between two versions of a file help you see the bug that was introduced?

I thought it was quite nice to see the diff, but I find it difficult to view
without colorcoding the different kinds of diffs. I will definetely use diff
commands when needed.

#### How could having easy access to the entire history of a file make you a more efficient programmer in the long term?

What I like about versioncontrol is that it feels a lot less scary to do big
code changes.


Earlier, I might have copied whole files or project many times throughout
development to keep an earlier working code available. The problem is that it
takes a lot of time to keep that tidy when there are multiple copies. One could
delete some old ones, but I could need them, even if I don't think so at the
time.

#### What do you think are the pros and cons of manually choosing when to create a commit, like you do in Git, vs having versions automatically saved, like Google Docs does?

The con is that you do need to remember to commit. Also you should commit at
reasonable points throughout your code, for instance after adding a feature, or
fixed a bug. A commit should be of only a single logical piece of code. A good
tip for making sure your commit is not too big is to describe everything the
commit is about in the commutmessage, and make that message into a single line.

A pro to manually choosing when to commit is that you are sure that you can
restore your code to a previous time, when you know that it is working. This can
help with debugging.

#### Why do you think some version control systems, like Git, allow saving multiple files in one commit, while others, like Google Docs, treat each file separately?

Git is meant for projects of code, so quite often, each file is related to
eachother. If one just restores one file, and keeps the rest of the files,
chances are tha the code will no longer work. Restore to a certain commit, which
would mean all files are restored to that point in time, the code would work
just like it did when the commit was made.

Google Docs however, only uses documents which do not normally relate to any
other file. One could easily write a letter to John Doe, make changes to a
spreadsheet of personal economy and a presentation for work, all within an
afternoon. None of them relate to eachother, so tracking them together makes no
sense.

#### How can you use the commands git log and git diff to view the history of files?

Use`git log` to view all commitmessages and their id. To also view how many
changes were made, use `git log --stat`. You can then browse through the history
untill you find what you need.

  To view differences between two commits, use `git diff <commitIDA>
  <commitIDB>`.

#### How might using version control make you more confident to make changes that could break something?

The barrier for making big changes to code is much smaller. Refactoring and
throwing away old unused code is not as dangerous anymore. We can do that and
test it afterwards, without risking losing a lot of time rewriting some older,
now lost, code from memory. Or we can see easily why the new code doesn't work,
  <!-- when viewing it side-by-side our old code.  -->
