# docker_images

[![GitHub](https://img.shields.io/github/license/alexenge/docker_images)](https://github.com/alexenge/docker_images/blob/r_basics/LICENSE)

Docker images as the basis for project-specific containers, ready to be used with the [Binder](https://mybinder.readthedocs.io/en/latest/introduction.html) cloud service

## R-based images

| Image                                                        | Included packages                                                                                                                                                                          |                                                                                                                                                                                                                            Status & demo                                                                                                                                                                                                                            |
| ------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | :-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
| [**`r_basics`**](https://hub.docker.com/r/alexenge/r_basics) | <ul><li>R + RStudio</li><li>R packages for mixed-effects modeling</li><li>R-papaja for APA-style manuscripts in R Markdown</li><li>Python (via Jupyter Notebook or R-reticulate)</li></ul> | [![GitHub Workflow Status (branch)](https://img.shields.io/github/workflow/status/alexenge/docker_images/autobuild/r_basics)](https://github.com/alexenge/docker_images/actions)<br>[![Docker Image Size (latest by date)](https://img.shields.io/docker/image-size/alexenge/r_basics)](https://hub.docker.com/r/alexenge/r_basics)<br>[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/alexenge/docker_images/r_basics?urlpath=rstudio) |
| [**`r_eeg`**](https://hub.docker.com/r/alexenge/r_eeg)       | <ul><li>Everything in `r_basics`</li><li>Python and R packages for EEG processing</li><li>The [hu-neuro-pipeline](https://github.com/alexenge/hu-neuro-pipeline)</li></ul>                 |       [![GitHub Workflow Status (branch)](https://img.shields.io/github/workflow/status/alexenge/docker_images/autobuild/r_eeg)](https://github.com/alexenge/docker_images/actions)<br>[![Docker Image Size (latest by date)](https://img.shields.io/docker/image-size/alexenge/r_eeg)](https://hub.docker.com/r/alexenge/r_eeg)<br>[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/alexenge/docker_images/r_eeg?urlpath=rstudio)       |
| [**`r_stan`**](https://hub.docker.com/r/alexenge/r_stan)     | <ul><li>Everything in `r_eeg`</li><li>The Stan language for probabilistic programming</li><li>Related R packages for Bayesian modeling</li></ul>                                           |     [![GitHub Workflow Status (branch)](https://img.shields.io/github/workflow/status/alexenge/docker_images/autobuild/r_stan)](https://github.com/alexenge/docker_images/actions)<br>[![Docker Image Size (latest by date)](https://img.shields.io/docker/image-size/alexenge/r_stan)](https://hub.docker.com/r/alexenge/r_stan)<br>[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/alexenge/docker_images/r_stan?urlpath=rstudio)     |

## Usage

After installing [Docker Desktop](https://www.docker.com/products/docker-desktop), the images can be pulled and run from [Docker Hub](https://hub.docker.com/u/alexenge):

```bash
docker run --rm -p 8888:8888 alexenge/r_basics:latest
```
