# CPMGEM Evaluation Notebooks

Evalution notebooks for "Machine learning emulation of precipitation from km-scale regional climate simulations using a diffusion model", a paper on ML approaches to emulate the Met Office's UK CPM precipitation output from UKCP Local, including introducing CPMGEM.
There are also further results for another paper, "Potential for machine learning emulators to augment regional climate simulations in provision of local climate change information", in `nbs/perspective-paper`.

## Setup

Assumes you have [pixi](https://pixi.sh) installed for managing dependencies.

1. Clone repo and cd into it
2. Install dependencies: `pixi install`
3. Create .env file: cp .env.example .env and then update to match your needs:
  * `DERIVED_DATA`: path to where derived data such datasets and model artefacts are kept

## Configuration

### Environment variables

Manage environment variables as you wish though the python-dotenv package is included for those wishing to use `.env` file.

| Name | Description |
|------|-------------|
|`DERIVED_DATA`| The common path to where datasets and emulator artefacts (including samples) are to be found |


## Usage

The notebooks can be run with Jupyter: `pixi run jupyter lab`
