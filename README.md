# Materialized GitHub Actions contexts by event type

Runs GitHub actions and dumps contexts to see what variables are available.
This can be helpful when writing GitHub actions workflows that use context variables.
Since the available context variables depend on the event type,
this repository aims to capture as many event types as possible.
Contributions are welcome to add additional event types.

## Contexts

Contexts are combined into a single JSON file and written back to the repository in the [`contexts`](contexts) directory.
The JSON files are also exported in [gron](https://github.com/tomnomnom/gron) format for easy identification of the absolute path to a value.

You can also search for workflow runs by event type:

- [push](https://github.com/dhimmel/dump-actions-context/actions?query=event:push)
- [pull_request](https://github.com/dhimmel/dump-actions-context/actions?query=event:pull_request)
- [workflow_dispatch](https://github.com/dhimmel/dump-actions-context/actions?query=event:workflow_dispatch)
- [schedule](https://github.com/dhimmel/dump-actions-context/actions?query=event:schedule)
- [release](https://github.com/dhimmel/dump-actions-context/actions?query=event:release)

One benefit of the workflow logs is that gron output has syntax highlighting.
However, workflow logs are only retained for 90 days,
so for many event types, only the materialized files committed back to the repository will be available.

## References

- https://docs.github.com/en/actions/learn-github-actions/contexts#example-printing-context-information-to-the-log
- https://github.com/community/community/discussions/12269
- https://twitter.com/dhimmel/status/1559592874282557442
