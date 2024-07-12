<h1 align="center">Enhancing Dense Distinct Query with Weighted Supervision for One-to-Many Matching in Detection Transformers</h1>



## Installation

Clone the source code from GitHub:

```bash
git clone https://github.com/JeixHuang/WDQ-DETR.git
cd WDQ-DETR
```

**Native Runner:** Setup a conda environment using [`conda`](https://github.com/conda/conda) / [`mamba`](https://github.com/mamba-org/mamba):

```bash
conda conda env create --file conda-recipe.yaml  # or `mamba env create --file conda-recipe.yaml`
```

This will automatically setup all dependencies.

**Containerized Runner:** Other than using the native machine with conda isolation, as an alternative, you can also use docker images to configure the environment.

Firstly, please follow [NVIDIA Container Toolkit: Installation Guide](https://docs.nvidia.com/datacenter/cloud-native/container-toolkit/install-guide.html) and [NVIDIA Docker: Installation Guide](https://docs.nvidia.com/datacenter/cloud-native/container-toolkit/install-guide.html#docker) to setup `nvidia-docker`.
Then you can run:

```bash
make docker-run
```

This command will build and start a docker container installed with proper dependencies.
The host path `/` will be mapped to `/host` and the current working directory will be mapped to `/workspace` inside the container.