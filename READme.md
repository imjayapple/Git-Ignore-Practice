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