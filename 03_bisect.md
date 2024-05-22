# Bisect - divide and conquer


A good place to start is [git-bisect](https://git-scm.com/docs/git-bisect)

## Basic commands
```bash
git bisect start
git bisect bad                     # Mark current version as bad
git bisect good v1.0.0-rc2         # v1.0.0-rc2 is known to be good
```

Once you set the good and the bad, git will select a commit in the middle and check it out.

```bash
# You compile, if it works type 
git bisect good

# if it does not compile
git bisect bad
```