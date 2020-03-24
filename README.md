# covid19-images

This monorepo includes forks of other projects which are building covid-related datasets. 

For examples, ieee8023 has collected positive CT scans. When you find a novel positive CT scan, submit a PR to ieee8023. When his repo is updated, this repo's subproject will syn with upstream and include that new image. 

In this way, datasets can be built modularly. Each dataset owner can validate, clean, and tag the images. This project focuses on aggregating, organizing, augmenting, and loading for use in models.
