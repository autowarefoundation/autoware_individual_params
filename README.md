# autoware_individual_params

This repository stores parameters that are different from each vehicle.

## Rationale

The parameters were originally managed in `launcher` repository.
Why we manage them in a separate repository are:

- Parameter maintainers don't require write-access to `launcher` repository.
- To rollback only parameters independently from `launcher`.
