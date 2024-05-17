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


## NANOAOD variable list

Each NANOAOD dataset has the variable list with a brief description attached to the portal record.

::::::::::::::::::::::::::::::::::::: challenge

## Challenge

Find the variable listings for a collision data record and a Monte Carlo data record. What are the differences? What is the same?

:::::::::::::::: solution

 - The data records have a "Luminosity" block with some beam related information whereas MC records have a "Runs" block with event generation information.
 - The MC records have event generator or simulation information in the "Events" block.
 - The variables of reconstructed objects, such as Muon, are the same for [data](https://opendata.cern.ch/eos/opendata/cms/dataset-semantics/NanoAOD/30563/SingleMuon_doc.html#Muon) and [MC](https://opendata.cern.ch/eos/opendata/cms/dataset-semantics/NanoAODSIM/35751/DYToMuMu_M-120To200_TuneCP5_13TeV-powheg-pythia8_doc.html#Muon).

:::::::::::::::::::::::::
:::::::::::::::::::::::::::::::::::::::::::::::

## Inspect datasets with ROOT

This part of the lesson will be done from within the [ROOT tools container](https://cms-opendata-workshop.github.io/workshopqcd-2024-lesson-docker/03-docker-for-cms-opendata.html#root-tools-container). You should have it available.
All ROOT commands will be typed inside that environment.

Work through the quick introduction to getting started with CMS NANOAOD Open Data in [the getting started guide page](https://opendata.cern.ch/docs/cms-getting-started-nanoaod) on the CERN Open Data portal.

:::::: checklist

### You will learn:

- [x] how to print out the event content of a NANOAOD file in ROOT
- [x] how to make a plot of a variable in the NANOAOD file with some selection criteria in ROOT

::::::::::::


## Inspect a dataset with python tools

This part of the lesson will be done from within the [python tools container](https://cms-opendata-workshop.github.io/workshopqcd-2024-lesson-docker/03-docker-for-cms-opendata.html#python-tools-container). You should have it available.
Open a new jupyter notebook from the jupyterlab tab that the container will open in your browser. Type the commands in code cells of the notebook.

First, import some python libraries:

```python
import uproot
import matplotlib.pylab as plt
import awkward as ak
import numpy as np
```

 - [uproot](https://uproot.readthedocs.io/en/latest/index.html) is a python inteface to ROOT
 - [matplotlib](https://matplotlib.org/) can be used for plotting
 - [numpy](https://numpy.org/) is a python package for scientific computing
 - [awkard](https://awkward-array.org/doc/main/) is a python library for variable-size data



### Print out event content with python tools



### Plot a variable with python tools


:::::: keypoints
- It's useful to inspect the files before diving into the full analysis.
- Some files may not have the information you're looking for.
::::::