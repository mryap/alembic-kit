Jupyter Notebooks designed to support
reproducible research. It enables data people to craft easily shared computational narratives that
mix code, results, and text [8, 9]. 

lower many barriers to reproducibility and were 


### List All Relevant Dependencies

Reproducing analysis will require accessing not only code, but also any
dependencies. I manage my dependencies
explicitly from the start with pip’s requirements.txt to list all relevant dependencies (including their software versions). 

Listing the versions of critical dependencies 
in the notebook itself (best done at the bottom) will ensure that, if used in isolation from its
environment, the notebook still contains critical information to help other replicate results.

In notebooks, you can use a notebook extension such
as [watermark](https://github.com/rasbt/watermark) to explicitly print out your dependencies. 

### Version Control

Jupyter Notebooks store both code and specialized and extensive
metadata about each cell as a text file in the JSON (JavaScript Object Notation) format. Version
control systems compare differences in these JSON files, not differences in the user-friendly
notebook GUI (graphical user interface). 

### Share Your Data

Ideally, share your entire dataset alongside your notebooks. I used the word ideally as many datasets
are too large or too sensitive to share this way.  Host public copies of medium-sized, anonymized data in 
figshare (https://figshare.com/), zenodo (https://zenodo.org/)).  These
hosting services provide Digital Object Identifiers (doi) to uniquely and permanently identify datasets, an important aspect of reproducibility. Having access to a clearly-annotated notebook is of little use to reproducibility if the underlying data is locked away.  

### Strive for Zero Installation 

Use Binder to provide a zero-install environment to run your notebooks in the cloud
(https://mybinder.org/) as community members would find installing Jupyter Notebook or Jupyter Lab a barrier to use. 
You can also create a Docker image of your environment (https://docs.docker.com/) to ease setup. 
