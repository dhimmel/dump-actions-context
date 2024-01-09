# dump-actions-context

Runs GitHub actions and dumps context to see what variables are available.

Search for workflow runs by event type:

- [push](https://github.com/dhimmel/dump-actions-context/actions?query=event:push)
- [pull_request](https://github.com/dhimmel/dump-actions-context/actions?query=event:pull_request)
- [workflow_dispatch](https://github.com/dhimmel/dump-actions-context/actions?query=event:workflow_dispatch)
- [schedule](https://github.com/dhimmel/dump-actions-context/actions?query=event:schedule)

Contexts are also combined into a single JSON file and written back to the repository in the [`contexts`](contexts) directory.

References:

- https://docs.github.com/en/actions/learn-github-actions/contexts#example-printing-context-information-to-the-log
- https://github.com/community/community/discussions/12269

