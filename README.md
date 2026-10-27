# allesfitter-tutorials

Fitting a light curve starts before the model call. The current walkthrough uses Lightkurve to retrieve a TESS product from MAST, trims it to the time, flux, and flux-uncertainty columns, then prepares a normalized CSV for Allesfitter. Start with [`Set-up/data_retrieval.ipynb`](Set-up/data_retrieval.ipynb) and update the TIC ID and output paths for your target.

Our `paths.py` module reads `ALLESFITTER_TUTORIALS_PATH`, which defaults to this checkout. It exposes local `data/` and `visuals/` directories. Git ignores both.

The path module uses TDpy's shared repository-path utility. Install its pinned version before running the tutorials.

```bash
python -m pip install "tdpy @ git+https://github.com/tansudaylan/tdpy.git@35df1703c6b63d6a62f7d44b12cf5928b5d355ed"
```
