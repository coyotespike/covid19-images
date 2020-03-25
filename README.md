# covid19-images

## Usage
Warning: a positive CT scan can diagnose the likely presence of COVID-19. Despite papers claiming the contrary, a negative scan means nothing.

You should use this data for machine learning research purposes, or in close collaboration with medical professionals in the ongoing prognosis and treatment of patients. Don't encourage policymakers to rely on CT scans as initial diagnosis.

https://lukeoakdenrayner.wordpress.com/2020/03/23/ct-scanning-is-just-awful-for-diagnosing-covid-19/

https://thehealthcareblog.com/blog/2020/03/23/can-ai-diagnose-covid-19-on-ct-scans-can-humans/

### Cloning
You will want the submodules' data as well.

`git clone --recursive git@github.com:coyotespike/covid19-images.git`

### Loader Scripts
Coming soon

We will include code to load data for TensorFlow, PyTorch, FastAI, and more, so that you can immediately start building your model.

Goal is one-liners that run a script so you can just jump into a Jupyter/Kaggle notebook.
## Purpose

PCR swabs are far more accurate than CT scans at diagnosing COVID-19, but CT scans can play a role in prognosis, treatment, and hospital decision-making. We need a large open-source dataset to enable many researchers/hackers to innovate, and to enable widespread usage of helpful AIs.

Deep learning in general works best with images. Many machine learning libraries require data to be organized in a certain way.

This project focuses on aggregating, organizing, augmenting, and loading data for use in models. We may have companion projects to directly source data.

## General Organization

This repo uses submodules to include forks of other projects which are building COVID-19-related datasets. 

For examples, ieee8023 has collected positive CT scans from academic papers. When you find a novel positive CT scan in an academic paper, submit a PR to ieee8023. When his repo is updated, this repo's subproject will sync with upstream and include that new image. 

In this way, datasets can be built modularly. Each dataset owner can validate, clean, and tag the images. 

## Contributing

Click on the [projects tab](https://github.com/coyotespike/covid19-images/projects/1) above to see what needs doing.

At this time (March 2020) Arterys Marketplace Slack is coordinating dataset aggregation. Get on there to get access to their Google documents where people are gathering datasets. I will remove this note if the center of gravity shifts elsewhere (or here) - Arterys is assisting deployment of AI models and datesets are a means to an end for them.

https://arterysmarket-6dm2046.slack.com/

## Adding an issue

Please assign to project `Covid19 Images Library` so that it is tracked more easily. PRs welcomed.
