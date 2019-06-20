# Git Hooks Demo

[Git Hooks Tutorials](https://www.atlassian.com/git/tutorials/git-hooks[)

# Change git hooks directory
By default the hooks directory is .git/hooks. But the .git/hooks directory isn’t cloned with the rest of your project, nor is it under version control. So maintaining hooks for a team of developers can be a little tricky. 

## Solution #1 Change core.hooksPath configration vriable.
Setting core.hooksPath configuration variable to hooks directory:
```bash
git config core.hooksPath .githooks
```

## Solution #2 Use symbolic links to link custom hooks to the ones in the .git/hooks folder