# `gh-workflow-test`

Test repo to experiment with different GHA workflow formats, the goal is:

  - A bunch of 'CI' steps that should run on each pushed commit to a PR, and
  - A 'deploy' job that runs only on commit on `main` and only if all the 'CI'
    steps also passed
