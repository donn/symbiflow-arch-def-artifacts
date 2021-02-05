# symbiflow-arch-def-artifacts
Manually assembled artifacts for known-workingish symbiflow-arch-defs.

# How they were created
All symbiflow-examples files are from commit [b0ee6d2](https://github.com/SymbiFlow/symbiflow-examples/commit/b0ee6d226410a5af56af9f636d0041c0e3a712ab).

## eos-s3
The artifacts were obtained from commit [71302a5](https://github.com/QuickLogic-Corp/quicklogic-fpga-toolchain/commit/71302a5e4b4122976ac9c6e90597146b93083525) of quicklogic's FPGA toolchain.

I built the `Dockerfile.use-installer` container then copied the definitions over.

The conda environment.yml is from https://github.com/SymbiFlow/symbiflow-examples, modified for a newer vtr.

## xc7 (Not working.)
Files obtained from download link in symbiflow-examples' documentation.

The file has been repackaged to include an `install/` directory to match eos-s3 and the environment.yml from the same commit. 

I'm not terribly focused on this one at the moment given the proprietary requirements.