# PR-test

_Testing Pull requests_

Create main repo (`i2i2t/PR-test`), then fork it (`camwebb/PR-test`).

``` 
git clone git@github.com:i2i2t/PR-test.git
mv PR-test PR-test-main
git clone git@github.com:camwebb/PR-test.git
mv PR-test PR-test-fork

cd PR-test-fork/
git branch new-file-branch
git switch new-file-branch
emacs new-file.md
git add new-file.md 
git commit -m "added new file" new-file.md
git push --set-upstream origin new-file-branch
```

Now go to `camwebb/PR-test` and switch to new-file-branch to see new
file. Create a pull request for `i2i2t/PR-test`). Review changes.

If you need to update the changed files in the PR:

```
cd PR-test-fork/
emacs new-file.md
git commit -m "edited new file" new-file.md
git push --set-upstream origin new-file-branch
```

These changes are automatically reflected in the PR in `i2i2t/PR-test`

Finally accept the Merge in `i2i2t/PR-test`.


