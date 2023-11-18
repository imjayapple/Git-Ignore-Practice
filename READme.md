A gitignore file specifies intentionally untracked files that Git should ignore. 

Files already tracked by Git are not affected.

Each line in a gitignore file specifies a pattern.

When deciding whether to ignore a path, Git normally checks gitignore patterns from multiple sources, with the following order of precedence, from highest to lowest (within one level of precedence, the last matching pattern decides the outcome)

What kind of files should you ignore?
• Log files
• Files with API keys/secrets, credentials, or sensitive information
• Useless system files like .DS_Store on macOS
• Generated files like dist folders
• Dependencies which can be downloaded from a package manager
• And there might be other reasons (maybe you make little todo.md files)

React examples:
# Created by https://www.toptal.com/developers/gitignore/api/react
# Edit at https://www.toptal.com/developers/gitignore?templates=react

### react ###
.DS_*
*.log
logs
**/*.backup.*
**/*.back.*

node_modules
bower_components

*.sublime*

psd
thumb
sketch

# End of https://www.toptal.com/developers/gitignore/api/react

Ignore Specific Directory:

Entire directories can be ignored, just include their paths, followed by a slash " / ":

ex.
GIT-IGNORE-PRACTICE/

Wildcard Operator:

"The * matches 0 or more characters (except the /).
So, for example, *.log matches any file ending with the .log extension

Negation

You can use a prefix of ! to negate a file that would be ignored.

ex.
*.log
!example.log

Important Note:
Any lines that start with # are comments, and these are very important when it comes to
keeping track of what files you are omitting and why.

ex.
# macOS Files
.DS_Store

# Node packages, do not commit
.node_modules