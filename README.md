# covid19-images

## Cloning
You will want the submodules' data as well.

`git clone --recursive git@github.com:coyotespike/covid19-images.git`
## Purpose

CT scans have proven more accurate than swab PCR tests for COVID-19. And the fastest test developed so far takes 45 minutes and is not widely deployed. CT scans with a good AI model will take 20 seconds.

To enable multiple methods of diagnosis, we should also build models (and secure accessible frontends) for x-rays - any data that lets a machine assist a human in diagnosing COVID-19.

Multiple teams are coming up with deep learning algorithms to diagnose COVID-19, but they have their own datasets. We need a large open-source dataset to enable many researchers/hackers to innovate, and to enable widespread usage of these AIs.

Deep learning in general works best with images. Many machine learning libraries require data to be organized in a certain way.

This project focuses on aggregating, organizing, augmenting, and loading data for use in models. We will include code to load data for TensorFlow, PyTorch, FastAI, and more, so that you can immediately start building your model.

## General Organization

This repo uses submodules to include forks of other projects which are building COVID-19-related datasets. 

For examples, ieee8023 has collected positive CT scans. When you find a novel positive CT scan, submit a PR to ieee8023. When his repo is updated, this repo's subproject will sync with upstream and include that new image. 

In this way, datasets can be built modularly. Each dataset owner can validate, clean, and tag the images. 

## Contributing

Click on the [projects tab](https://github.com/coyotespike/covid19-images/projects/) above to see what needs doing.
