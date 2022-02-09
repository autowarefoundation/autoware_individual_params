# autoware_individual_params

This repository stores parameters that are different from each vehicle.

## Rationale

The parameters were originally managed in `launcher` repository.
Why we manage them in a separate repository are:

- Parameter maintainers don't require write-access to `launcher` repository.
- To rollback only parameters independently from `launcher`.

## Directory Structure

```shell
individual_params/
├── config
│   └── default # vehicle id
│       ├── aip_x1 # sensor name
│       │   ├── sensor_kit_calibration.yaml
│       │   ├── sensors_calibration.yaml
│       │   └── ... # other settings
│       └── aip_xx1 # sensor name
│           └── ... # some settings
├── CMakeLists.txt
└── package.xml
```
