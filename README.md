# covid19-images

## Usage
Warning: a positive CT scan can diagnose the likely presence of COVID-19. Despite papers claiming the contrary, a negative scan means nothing.

https://lukeoakdenrayner.wordpress.com/2020/03/23/ct-scanning-is-just-awful-for-diagnosing-covid-19/

You should use this data for machine learning research purposes, or in close collaboration with medical professionals. Don't encourage policymakers to rely on CT scans as initial diagnosis.

### Cloning
You will want the submodules' data as well.

`git clone --recursive git@github.com:coyotespike/covid19-images.git`

### Loader Scripts
Coming soon

We will include code to load data for TensorFlow, PyTorch, FastAI, and more, so that you can immediately start building your model.

Goal is one-liners that run a script so you can just jump into a Jupyter/Kaggle notebook.
## Purpose

CT scans have proven more accurate than swab PCR tests for COVID-19. And the fastest test developed so far takes 45 minutes and is not widely deployed. CT scans with a good AI model will take 20 seconds.

To enable multiple methods of diagnosis, we should also build models (and secure accessible frontends) for x-rays - any data that lets a machine assist a human in diagnosing COVID-19.

Multiple teams are coming up with deep learning algorithms to diagnose COVID-19, but they have their own datasets. We need a large open-source dataset to enable many researchers/hackers to innovate, and to enable widespread usage of these AIs.

Deep learning in general works best with images. Many machine learning libraries require data to be organized in a certain way.

This project focuses on aggregating, organizing, augmenting, and loading data for use in models. We may have companion projects to directly source data.

## General Organization

This repo uses submodules to include forks of other projects which are building COVID-19-related datasets. 

For examples, ieee8023 has collected positive CT scans. When you find a novel positive CT scan, submit a PR to ieee8023. When his repo is updated, this repo's subproject will sync with upstream and include that new image. 

In this way, datasets can be built modularly. Each dataset owner can validate, clean, and tag the images. 

## Contributing

Click on the [projects tab](https://github.com/coyotespike/covid19-images/projects/1) above to see what needs doing.

At this time (March 2020) Arterys Marketplace Slack is coordinating dataset aggregation. Get on there to get access to their Google documents where people are gathering datasets. I will remove this note if the center of gravity shifts elsewhere (or here) - Arterys is assisting deployment of AI models and datesets are a means to an end for them.

https://arterysmarket-6dm2046.slack.com/

## Adding an issue

Please assign to project `Covid19 Images Library` so that it is tracked more easily. PRs welcomed.
