[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-v2.0%20adopted-ff69b4.svg)](code_of_conduct.md)

# covid19-images

## Usage
Warning: a positive CT scan can diagnose the likely presence of COVID-19. Despite papers claiming the contrary, a negative scan means nothing.

You should use this data for machine learning research purposes, or in close collaboration with medical professionals in the ongoing prognosis and treatment of patients. Don't encourage policymakers to rely on CT scans as initial diagnosis.

https://lukeoakdenrayner.wordpress.com/2020/03/23/ct-scanning-is-just-awful-for-diagnosing-covid-19/

https://thehealthcareblog.com/blog/2020/03/23/can-ai-diagnose-covid-19-on-ct-scans-can-humans/

### Loader Scripts
Coming soon

We will include code to load data for TensorFlow, PyTorch, FastAI, and more, so that you can immediately start building your model.

Goal is one-liners that run a script so you can just jump into a Jupyter/Kaggle notebook.

This means we will also assemble usable datasets.

## Purpose

PCR swabs are far more accurate than CT scans at diagnosing COVID-19, but CT scans can play a role in prognosis, treatment, and hospital decision-making. We need a large open-source dataset to enable many researchers/hackers to innovate, and to enable widespread usage of helpful AIs.

Deep learning in general works best with images. Many machine learning libraries require data to be organized in a certain way.

This project focuses on aggregating, organizing, augmenting, and loading data for use in models. A couple of the submodules also directly source data.

## General Organization

We want to include the unprocessed data, so that anyone can drop down and process the data any way they want.

At the second layer, we will include minimally processed data - for instance turning JPEG into DICOM files.

Finally, we will include fully assembled datasets for CT scans and for x-rays, in test/train/val folders, ready to use in any machine learning library.

This repo uses submodules to include forks of other projects which are building COVID-19-related datasets. 

For examples, ieee8023 has collected positive CT scans from academic papers. When you find a novel positive CT scan in an academic paper, submit a PR to ieee8023. When his repo is updated, this repo's subproject will sync with upstream and include that new image. 

In this way, datasets can be built modularly. Each dataset owner can validate, clean, and tag the images. 

## Folder Contents

### COVID-positive CT Scans
- [AH Paris](https://github.com/coyotespike/AHP-covid19-ctscans)
- [ieee8023's dataset](https://github.com/coyotespike/covid-chestxray-dataset)

### COVID-positive x-rays
- [ieee8023's dataset](https://github.com/coyotespike/covid-chestxray-dataset)

### COVID-negative x-rays
- [Zhang Lab](https://github.com/coyotespike/zhanglab-chest-xrays/) - these include normal and pneumonia x-rays.
- [NIH Sample](https://github.com/coyotespike/NIH-chestxray-dataset-sample)

### Unknown
- [covid-19-pos-case](https://github.com/coyotespike/covid-19-pos-case) - nothing is known about this data at present

### Datasets
#### x-rays
- [Darshan Deshpande's dataset](https://github.com/coyotespike/covid19-detection-xray-dataset)

#### CT Scans
- None yet

## Contributing

Click on the [projects tab](https://github.com/coyotespike/covid19-images/projects/1) above to see what needs doing.

## Adding an issue

Please assign to project `Covid19 Images Library` so that it is tracked more easily. PRs welcomed.
