# symbiflow-arch-def-artifacts
Manually assembled artifacts for known-workingish symbiflow-arch-defs, aiming for compatibility with [silkflow](https://github.com/efabless/silkflow).

# How they were created
All symbiflow-examples files are from commit [b0ee6d2](https://github.com/SymbiFlow/symbiflow-examples/commit/b0ee6d226410a5af56af9f636d0041c0e3a712ab).

## ice40
Artifacts built from repository https://github.com/symbiflow/symbiflow-arch-defs commit [ce80f99](https://github.com/symbiflow/symbiflow-arch-defs/commit/ce80f998bdf66d6c2083f9de28441aab008bb67d) and copied over.

environment.yml and requirements.txt created manually.

## xc7
From symbiflow-examples pretty much verbatim. The file has been repackaged to include an `install/` directory to match ice40/eos-s3 and the environment.yml from the same commit. 

environment.yml and requirements.txt were also included in the package to be silkflow compatible.

Scripts have been removed.

## eos-s3
The artifacts were obtained from commit [71302a5](https://github.com/QuickLogic-Corp/quicklogic-fpga-toolchain/commit/71302a5e4b4122976ac9c6e90597146b93083525) of quicklogic's FPGA toolchain.

I built the `Dockerfile.use-installer` container then copied the definitions over.

The conda environment.yml is from symbiflow-examples, modified for a newer vtr.

eos-s3 is not currently Silkflow compatible. As quicklogic kind of went their own way with the toolchain.
