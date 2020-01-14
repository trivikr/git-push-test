# git-push-test

* Verified that solution provided by [GitHub documentation](https://help.github.com/en/github/using-git/dealing-with-non-fast-forward-errors) works in [trivikr/git-push-test](https://github.com/trivikr/git-push-test) repo
* Commands run while testing:
  * git tag &lt;tag&gt; &lt;commit&gt; -m &lt;tag&gt;
  * git fetch origin
  * git merge origin master -m "&lt;commit-msg&gt;"
  * git push
  * git push --tags
* Commits
  * [local commit testing fast-forward merge](https://github.com/trivikr/git-push-test/commit/58ae6f51b873ed8136e8d87ec975d230003a8690)
  * [remote commit to create non-fast-forward error](https://github.com/trivikr/git-push-test/commit/2ab017052dd35558673bfa18e88f4c57d43ce9f9)
  * [merge commit](https://github.com/trivikr/git-push-test/commit/59b60e256588cd110248094d73ad2a8b577decd0)
* Verification:
  * Tag `fast-forward-merge` has only local commit ([commits](https://github.com/trivikr/git-push-test/commits/fast-forward-merge))
  * Tag `no-remote-updates` has no merge commits ([commits](https://github.com/trivikr/git-push-test/commits/no-remote-updates)) created while pushing [d1cc0272f56eb53d97c174c5deab0d652936a201](https://github.com/trivikr/git-push-test/commit/d1cc0272f56eb53d97c174c5deab0d652936a201)
