# **GIT  :**

Git comes with a tool called git config that lets you get and set configuration variables that control
all aspects of how Git looks and operates. These variables can be stored in three different places:
1. /etc/gitconfig file: Contains values applied to every user on the system and all their
repositories. If you pass the option --system to git config, it reads and writes from this file
specifically. (Because this is a system configuration file, you would need administrative or
superuser privilege to make changes to it.)
2. ~/.gitconfig or ~/.config/git/config file: Values specific personally to you, the user. You can
make Git read and write to this file specifically by passing the --global option, and this affects
all of the repositories you work with on your system.
3. config file in the Git directory (that is, .git/config) of whatever repository you’re currently
using: Specific to that single repository. You can force Git to read from and write to this file with
the --local option, but that is in fact the default. (Unsurprisingly, you need to be located
somewhere in a Git repository for this option to work properly.)
Each level overrides values in the previous level, so values in .git/config trump those in
/etc/gitconfig.

### **GIT COMMANDS :**
```
Main Porcelain Commands
   add                  Add file contents to the index
   am                   Apply a series of patches from a mailbox
   archive              Create an archive of files from a named tree
   bisect               Use binary search to find the commit that introduced a bug
   branch               List, create, or delete branches
   bundle               Move objects and refs by archive
   checkout             Switch branches or restore working tree files
   cherry-pick          Apply the changes introduced by some existing commits
   citool               Graphical alternative to git-commit
   clean                Remove untracked files from the working tree
   clone                Clone a repository into a new directory
   commit               Record changes to the repository
   describe             Give an object a human readable name based on an available ref
   diff                 Show changes between commits, commit and working tree, etc
   fetch                Download objects and refs from another repository
   format-patch         Prepare patches for e-mail submission
   gc                   Cleanup unnecessary files and optimize the local repository
   gitk                 The Git repository browser
   grep                 Print lines matching a pattern
   gui                  A portable graphical interface to Git
   init                 Create an empty Git repository or reinitialize an existing one
   log                  Show commit logs
   merge                Join two or more development histories together
   mv                   Move or rename a file, a directory, or a symlink
   notes                Add or inspect object notes
   pull                 Fetch from and integrate with another repository or a local branch
   
   ```
   ```
   The rules for the patterns you can put in the .gitignore file are as follows:
• Blank lines or lines starting with # are ignored.
• Standard glob patterns work, and will be applied recursively throughout the entire working
tree.
• You can start patterns with a forward slash (/) to avoid recursivity.
• You can end patterns with a forward slash (/) to specify a directory.
• You can negate a pattern by starting it with an exclamation point (!).
Glob patterns are like simplified regular expressions that shells use. An asterisk (*) matches zero or
more characters; [abc] matches any character inside the brackets (in this case a, b, or c); a question
mark (?) matches a single character; and brackets enclosing characters separated by a hyphen 
([0-9]) matches any character between them (in this case 0 through 9).
You can also use two asterisks to match nested directories; a/**/z would match a/z, a/b/z, a/b/c/z, and so on.
```
