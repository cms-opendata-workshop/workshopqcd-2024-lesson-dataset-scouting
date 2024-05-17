---
title: "What is in the datafiles?"
teaching: 5
exercises: 5
---

:::::: questions
- How do I inspect these files to see what is in them?

::::::

:::::: objectives
- To be able to see what objects are in the data files

::::::

In the following, we will learn about CMS data in the NANOAOD format. This is the data format
that can be accessed without CMS-specific software using ROOT or python tools.

A part of this lesson will be done from within the [ROOT tools container](https://cms-opendata-workshop.github.io/workshopqcd-2024-lesson-docker/03-docker-for-cms-opendata.html#root-tools-container). You should have it available.
All commands will be typed inside that environment.

## NANOAOD variable list

Each NANOAOD dataset has the variable list with a brief description attached in the portal record.

## Inspect datasets with ROOT

Work through the quick introduction to getting started with CMS NANOAOD Open Data in [the getting started guide page](https://opendata.cern.ch/docs/cms-getting-started-nanoaod) on the CERN Open Data portal.

:::::: checklist

### You will learn:

- [x] how to print out the event content of a NANOAOD file in ROOT
- [x] how to make a plot of a variable in the NANOAOD file with some selection criteria in ROOT

::::::::::::


## Inspect dataset with python tools



:::::: keypoints
- It's useful to inspect the files before diving into the full analysis.
- Some files may not have the information you're looking for.
::::::