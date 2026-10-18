This repository contains the report and code for my undergraduate research project, completed with Joseph Tarr under the supervision of Professor Jeffrey Giansiracusa at Durham University.

We tackle ligand-based virtual screening: predicting whether a molecule will bind to a given protein target. The novel idea in our approach is representing each molecule through multiple viewpoints: we render it as isometric projections from several positions on a surrounding sphere and pass every view through a shared convolutional neural network. For each learned feature, we then take the maximum across all views, so the most informative viewpoint determines the prediction. This approximates rotational invariance. On the AKT1 target from the DUD-E dataset, using six views per molecule improved our validation AUROC from 0.72 to 0.84 compared with a single view.

My main contribution is the model described in Chapter 3.

[📄 Machine Learning for Drug Discovery (PDF)](https://github.com/user-attachments/files/33627390/Machine_Learning_for_Drug_Discovery.30.pdf)

Model.ipynb contains my code for the model, the training loop, and validation. It takes unnormalised image data as a tensor input.
