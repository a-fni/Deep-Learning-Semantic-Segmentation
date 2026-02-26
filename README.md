# Deep Learning Semantic Segmentation

This repository contains the second project assignment of the [Artificial Neural Networks and Deep Learning](https://onlineservices.polimi.it/manifesti/manifesti/controller/ManifestoPublic.do?EVN_DETTAGLIO_RIGA_MANIFESTO=evento&aa=2025&k_cf=225&k_corso_la=542&k_indir=T2I&codDescr=054307&lang=IT&semestre=1&anno_corso=2&idItemOfferta=180465&idRiga=340586)
course at Politecnico di Milano.

## Overview

The objective of this assignment was to build a deep learning model able to perform semantic segmentation of $64x128$ images of mars' surface.
The entire code base, which includes data loading, preprocessing, augmentation, model definition, training and evaluation is contained in a Python notebook since development
occurred on [Google Colab](https://colab.research.google.com/).

Development time was 2 weeks, involved a team of 4 people and the final obtained score was **5.5 out of 5.5** points. On top of the full source code a final report of at most 3 pages
was also submitted documenting decisions, the full development process and final model evaluation.

The training set provided included a total of 2,615 greyscale samples and can be found under `source/mars/`. Because of its size, the training set has been split into multiple 50MiB partitions
which can be combined into the original full training set by running:

```bash
cat mars.npz.part_a* >> mars.npz
```

Any other relevant information regarding the model, its development and performance can be found in the final report handed in which can
be found under the `delivery/` directory. 
