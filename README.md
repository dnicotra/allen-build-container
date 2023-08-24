# allen-build-container
Apptainer/Singularity DEF file to build LHCb Allen (Standalone, CUDA or CPU).

## Info
Based on `nvidia/cuda:11.8.0-devel-ubuntu22.04`

## Instructions
0. (Optional) Customize the base image to match your CUDA configuration. [Pick the right tag here](https://hub.docker.com/r/nvidia/cuda/tags?page=1&name=devel-ubuntu22.04).
1. Build the image
```
apptainer build allen.sif allen.def
```
3. Run the image
```
apptainer run --nv allen.sif
```

## Notes
- Tested on Nikhef's Stoomboot node wn-lot-008
