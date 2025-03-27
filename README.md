# CPMGEM Evaluation Notebooks

Evalution notebooks for "Machine learning emulation of precipitation from km-scale regional climate simulations using a diffusion model", a paper on ML approaches to emulate the Met Office's UK CPM precipitation output from UKCP Local, including introducing CPMGEM.

## Setup

This guide assumes you are using conda (or mamba) to manage packages and python environments.

1. Install conda environment:
  * If you wish to re-use the exact environment: `conda env create --file environment.lock.yml` and activate it: `conda activate cpmgem-pr-paper`
  * OR install the needed conda and pip packages to your own environment: `conda install --file=environment.txt`
2. Create .env file: cp .env.example .env and then update to match your needs:
  * `DERIVED_DATA`: path to where derived data such datasets and model artefacts are kept

## Configuration

### Environment variables

Manage environment variables as you wish though the python-dotenv package is included for those wishing to use `.env` file.

| Name | Description |
|------|-------------|
|`DERIVED_DATA`| The common path to where datasets and emulator artefacts (including samples) are to be found |


## Usage

The notebooks can be run with Jupyter: `jupyter lab`
