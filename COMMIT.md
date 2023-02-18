# Simple Conventional Commits

## Summary

The Conventional Commits specification is a lightweight convention on top of commit messages. It provides an easy set of rules for creating an explicit commit history; which makes it easier to write automated tools on top of. This is a simplified version, you can find the complete guide by checking the links in reference section.

## Commit structure

The commit contains the following structural elements, to communicate intent to the consumers of your library:

```
feat: add hat wobble
^--^  ^------------^
|     |
|     +-> Summary in imperative.
|
+-------> Type: chore, docs, feat, fix, refactor, or test.

[optional body]

[optional footer]
```

- `feat`: Introduces a new feature to the codebase (correlates with MINOR in SemVer)
- `fix`: Patches a bug in your codebase (equivalent to PATCH in Semantic Versioning)
- `docs`: Changes to the documentation
- `refactor`: Refactoring production code, eg. renaming a variable, changing code style, etc
- `test`: Adding missing tests, refactoring tests; no production code change
- `chore`: Indicate updates to build tasks, admin settings, packages, etc; no production code change
- `BREAKING CHANGE`: Must be added to the footer whenever a commit introduces a breaking API change (correlating with MAJOR in Semantic Versioning). A BREAKING CHANGE can be part of commits of any type

## Rules
- Always lowercased; except for nouns and special words
- Emojis are only allowed at the end of first line, right after the summary
- If a commit needs to use more than one type you should go back and make multiple commits when possible, otherwise use the `|` (pipe) symbol to split them, eg: `feat|fix`

## References

- https://gist.github.com/joshbuchea/6f47e86d2510bce28f8e7f42ae84c716
- https://www.conventionalcommits.org/
- https://seesparkbox.com/foundry/semantic_commit_messages
- http://karma-runner.github.io/1.0/dev/git-commit-msg.html
- https://github.com/qoomon/git-conventional-commits