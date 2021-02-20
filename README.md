# turbo-set-plot-waterfall-bug-demo

This is a demo of https://github.com/UCBerkeleySETI/turbo_seti/issues/188

`plot_event_pipeline` runs successfully and generates `.png` outputs, but does not show the plots inline in the notebook.

## Run on Binder

**Upstream version** (broken)
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/OliverEvans96/turbo-seti-waterfall-plot-bug-demo/main?filepath=demo.ipynb)

**My version** (working, patched with https://github.com/UCBerkeleySETI/turbo_seti/pull/187)
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/OliverEvans96/turbo-seti-waterfall-plot-bug-demo/patched?filepath=demo.ipynb)

## Run locally
1. Download my bug demo locally from https://github.com/OliverEvans96/turbo-seti-waterfall-plot-bug-demo

```bash
# Clone the repo
git clone https://github.com/OliverEvans96/turbo-seti-waterfall-plot-bug-demo.git
```

2. Create, and activate the conda env

```bash
# Create the environment from the definition file
conda env create -f environment.yml

# Activate the new environment
conda activate turbo_seti_waterfall_bug

# Create a Jupyter kernel for this environment to make it accessible from a notebook
python -m ipykernel install --user --name=turbo_seti_waterfall_bug
```

3. Start a Jupyter server and open `demo.ipynb`
4. Select the `turbo_seti_waterfall_bug` kernel (Kernel > Change Kernel)
5. Run all cells
