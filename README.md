# `gh-workflow-test`

Test repo to experiment with different GHA workflow formats, the goal is:

  - A bunch of 'CI' steps that should run on each pushed commit to a PR, and
  - A 'deploy' job that runs only on commit on `main` and only if all the 'CI'
    steps also passed

Examples:

  - [PR with all checks
    passing](https://github.com/matthewhughes-uw/gh-workflow-test/pull/2) note
    the `deploy` step is shown in the list of actions (though it is skipped)
  - [PR with a failing
    check](https://github.com/matthewhughes-uw/gh-workflow-test/pull/3)
  - [commit on `main` that
    deployed](https://github.com/matthewhughes-uw/gh-workflow-test/actions/runs/9079794163)
  - [commit on `main` that failed
    tests](https://github.com/matthewhughes-uw/gh-workflow-test/actions/runs/9079804420)
    the change was not deployed

See also:

  - [`74d9fa46a15f4293499e0ee1b3da376f6c7c83d3`](https://github.com/matthewhughes-uw/gh-workflow-test/commit/74d9fa46a15f4293499e0ee1b3da376f6c7c83d3):
    adding a job output and passing it down to the deploy step
