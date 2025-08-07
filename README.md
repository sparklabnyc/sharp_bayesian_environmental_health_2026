# SHARP: Bayesian Modeling for Environmental Health Workshop

![](assets/bmeh-1200x630.jpg)

## Introduction

GitHub repo through which we're developing and sharing materials for the SHARP Bayesian Modeling for Environmental Health Workshop, taking place in person during August 14th-15th 2025.

## Notes for attendees

The workshop will be a series of lectures and interactive supervised lab sessions. We hope it's informative and fun!

We will be using `Posit (RStudio) Cloud`, which assumes knowledge of `R` and `RStudio`. We will also ask you to pull the final versions of the `GitHub` repo to your Cloud account. The basics of doing this are in a previously-created guide found via [another guide repo](https://github.com/rmp15/rstudio_cloud_tutorial/tree/main).

This workshop is largely written in [`NIMBLE`](https://r-nimble.org/). There are also several elements in [`R-INLA`](https://www.r-inla.org/).

Below is the set of labs to follow throughout the two days:

### Day 1 (August 14th 2025)

| Time | Activity |
|----|----|
| 8:30 - 9:00 | Check in and breakfast |
| 9:00 - 9:15 | [Welcome and introduction](/lectures/welcome_and_introduction/welcome_and_introduction.qmd) |
| 9:15 - 10:00 | [Principles of Bayesian statistics](/lectures/principles_of_bayesian_statistics/principles_of_bayesian_statistics.qmd) (Lecture) |
| 10:00 - 10:15 | Break |
| 10:15 - 11:00 | [Principles of Bayesian statistics](/labs/principles_of_bayesian_statistics/principles_of_bayesian_statistics.qmd) (Hands-on Lab) |
| 11:00 - 11:15 | Break |
| 11:15 - 12:00 | [Bayesian workflow](/lectures/bayesian_workflow/bayesian_workflow.qmd) (Lecture) |
| 12:00 - 1:00 | Lunch |
| 1:00 - 1:45 | [Hierarchical modeling](/lectures/hierarchical_modelling/hierarchical_modelling.qmd) (Lecture) |
| 1:45 - 2:00 | Break |
| 2:00 - 2:45 | [Hierarchical modelling](/labs/hierarchical_modelling/hierarchical_modelling.qmd) (Hands-on Lab) |
| 2:45 - 3:00 | Questions and wrap-up |
| 3:00 - 3:45 | [Non-linear regression](/lectures/non_linear_regression/non_linear_regression.qmd) (Lecture) |
| 3:45 - 4:00 | Break |
| 4:00 - 4:45 | [Non-linear regression](/labs/non_linear_regression/non_linear_regression.qmd) (Hands-on Lab) |
| 4:45 - 5:00 | Questions and wrap-up |

### Day 2 (August 15th 2025)

| Time | Activity |
|----|----|
| 8:30 - 9:00 | Check in and breakfast |
| 9:00 - 10:00 | [Spatial and spatio-temporal modeling](/lectures/spatial_and_spatiotemporal_modeling/spatial_and_spatiotemporal_modeling.qmd) (Lecture) |
| 10:00 - 10:15 | Break |
| 10:15 - 11:00 | [Spatial and spatio-temporal modelling](/labs/spatial_and_spatiotemporal_modeling/spatial_and_spatiotemporal_modeling.qmd) (Hands-on Lab) |
| 11:00 - 11:15 | Break |
| 11:15 - 12:00 | [Software options](lectures/software_options/software_options.qmd) (Lecture) |
| 12:00 - 1:00 | Lunch |
| 1:00 - 1:45 | [Software options](/labs/software_options/software_options.qmd) (Hands-on Lab) |
| 1:45 - 2:00 | Break |
| 2:00 - 2:45 | [Advanced models](lectures/advanced_models/advanced_models.qmd) (Lecture) |
| 2:45 - 3:00 | Break |
| 3:00 - 3:45 | [Advanced models](/labs/advanced_models/advanced_models.qmd) (Hands-on Lab) |
| 3:45 - 4:30 | Interactive panel discussion & course wrap-up |
| 4:30 - 5:00 | Final farewell |

## Notes for those working on the repo

### Using `pre-commit`

Run `pre-commit install` to install the hooks. You now won't be able to commit until you pass the hooks. These (among other things) automatically format files and prevent us from committing ugly code. For more details, see the main [docs](https://pre-commit.com/) and the `R` [docs](https://lorenzwalthert.github.io/precommit/).

### Using `renv`

`renv` maintains consistency between users' `R` environments. Run `renv::restore()` and the environment will be downloaded into the repository based on the `renv.lock` file. If you want to add a packages to the lockfile, install the package and then run `renv::snapshot()`. For more details, see the [docs](https://rstudio.github.io/renv/articles/renv.html).

### Using `Quarto` for presentations

Quarto is pretty cool. I won't bore you, but have a look at the [docs](https://quarto.org/docs/guide/). Here, we're using it for [presentations](https://quarto.org/docs/presentations/revealjs/). It's designed by the folks at `RStudio`, so you `R` folk will be happy. Make a `.qmd` file and run `quarto render *.qmd` to generate the `html`, which you can open in browser. We can get fancy and import our own `css` to have a consistent theme for out presentations.
