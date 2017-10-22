# Lerna sample repo

## Publish

```bash
# just increment version
lerna publish --skip-git

# inc version of all changes packages
# set tag on git
# push to git origine
lerna publish

# inc version of all changes packages
# set tag on git
# push to git origine
lerna publish -m "chore(release): publish %s"
```

## Cleanup

```bash
lerna clean
```

## Git Commit Msg

See also: https://seesparkbox.com/foundry/semantic_commit_messages

Format of the commit message:

```html
<type>(<scope>): <subject>

<body>

<footer>
```

Allowed <type> values:

* feat (new feature)
* fix (bug fix)
* docs (changes to documentation)
* style (formatting, missing semi colons, etc; no code change)
* refactor (refactoring production code)
* test (adding missing tests, refactoring tests; no production code change)
* chore (updating grunt tasks etc; no production code change)

Example <scope> values:
* init
* runner
* watcher
* config
* web-server
* proxy
* etc.

The ```<scope>``` can be empty (eg. if the change is a global or difficult to assign to a single component), in which case the parentheses are omitted.
