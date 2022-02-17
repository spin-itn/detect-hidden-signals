# detect-hidden-signals
Functions to extract coherence matrices from DAS data and perform unsupervised classification on them

The algorithm to extract coherence matrices follows the method described in "Detecting seismic activity with a covariance matrix analysis of data recorded on seismic arrays" by L. Seydoux, N.M. Shapiro, J. de Rosny, F. Brenguier, M. Landès; in Geophysical Journal International, 2016;  DOI: [https://doi.org/10.1093/gji/ggv531](https://doi.org/10.1093/gji/ggv531)

Contrary to other approaches, we average coherence matrices over a frequency band, perform a dimensionality reduction using PCA and then run an agglomerative clustering algorithm on the reduced set of features. The advantage is that with PCA we can reconstruct a covariance matrix from the reduced feature set. This allows to identify noise sources in space in time.

If you use this code, we would appreciate a citation: DOI: [10.5281/zenodo.6123047](https://doi.org/10.5281/zenodo.6123047)

This is a static version of the code. For an up-to-date version, please check the repository on Julius Grimm's github: [jgrimm / detect-hidden-signals](https://github.com/jgrmm/detect-hidden-signals).
