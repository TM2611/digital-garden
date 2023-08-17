---
---

# Stop tracking changes for files already in the repository

# Encounter Detail
[<sub><sup>Write a detailed description of the problem you encountered here. Include any error messages, unexpected behaviours, and the context in which the problem occurred.</sup></sub>]

Tried to add all subfolders with the name `.obsidian` to `.gitignore`. 

```javascript
#.gitignore

**/.obsidian/
```

 .obsidian was already tracked by git before it was added to the `.gitignore` file, so git continued to track changes. Adding a file or folder to `.gitignore` will prevent untracked files from being added to the set of files that git manages, but it does not stop git from tracking already tracked files.

You can confirm if this is the case by running `git ls-files --cached | grep .obsidian`. If any files show up, they are still tracked by git.

## # Solution
[<sub><sup>Explain the solution that was implemented to resolve the problem. Include the steps you took, the resources you used, and any important learnings you want to highlight.</sup></sub>]

```bash
// You can include code snippets like this
git rm --cached -r personal/.obsidian
```

The `-r` option is to recursively remove files in that directory. `--cached` means only remove files from the index (i.e., stop tracking them), but do not remove them from the filesystem.

Once committed, git stopped showing diffs for files in the `personal/.obsidian` directory.

Do note that this will remove those files from the current branch and any other branch that merges these changes. So use it carefully.


#encounter

[[Software Development MOC]]