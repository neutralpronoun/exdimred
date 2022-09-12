# ExDimRed
### Examples for Dimensionality Reduction

ExDimRed is a simple visualisation tool, aimed and understanding and evaluating dimensionality reduction methods, using human-intuitive examples.

Examples are 3D point data which are reduced via dimensionality reduction methods to 2D.

### Usage

Novel methods, or methods not encluded by default, should follow the standard Scikit-Learn syntax, i.e. have the methods

`model.fit_transform(X)` to fit to and project input data `X`.

ExDimRed is accessed as follows:

```
from sklearn.manifold import Isomap
from exdimred import run

run(Isomap)
```

This will attempt to generate a pdf of the visualisation in the root directory.
If pdf generation fails then a png is generated instead.

### Requirements

ExDimRed requires `Python >= 3.8` and the packages `numpy`, `matplotlib`, `scikit-learn`, and `umap-learn` to be installed.

