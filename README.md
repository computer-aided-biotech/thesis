# EXCLAIMER: never mind all of the following requirements, all data can be found in the data folder



# Masters Thesis Jonas Sindlinger

Analysis of protoemics data from this paper: https://doi.org/10.1038/nbt.3418


## Requirements

* Python 3 
* R
* Git (or any Git client of your choice, e.g. [Github Desktop](https://desktop.github.com/))

## Installation


 this should in the future be running a docker container
* install docker if not already done
* navigate to this file in the console and run:
``` bash
docker-compose run --service-ports notebook
```
* after building a command prompt should open allowing you to open jupyter-notebooks
* to open a jupyter notebook run 
```bash
jupyter-notebook --allow-root
```


## Repository Structure

    |- data science
    |  |- code/            # all programmatic code relating to the project
    |  |   +- templates/    # scripts for generating template files
    |  |
    |  |- data/            # all data from the study
    |  |  |- raw_internal/ # raw data generated in-lab or by collaborators, will not be altered
    |  |  |- raw_external/ # data from third-party sources, databases etc, will not be altered
    |  |  |- intermediate/ # intermediate data on its way from raw to final
    |  |  +- final/        # final data for figures/visualizations
    |  | 
    |  |- results          # all output from workflows and analyses
    |     |- figures/      # graphs, likely designated for manuscript figures
    |     +- pictures/     # diagrams, images, and other non-graph graphics
    |
    |- doc/             # documentation for the study and other explanatory material
    |
    |
    |- .env             # file to store passwords and usernames needed for the scripts. This
    |                     will not get synced to GitHub.
    |- .gitignore       # files that will not sync to Github
    |- LICENSE          # license
    |- README.md        # the top level description of content
    |- requirements.txt # the requirements file for reproducing the analysis environment,
    |                     e.g. generated with `pip freeze > requirements.txt`
    +- to-dos.md        # pending things that are yet to be done

Navigate to each folder's `README.md` to learn more about the corresponding section.

## Acknowledgments

The initial file and directory structure of this project was developed by a group of participants in the Reproducible Science Curriculum Workshop, held at [NESCent] in December 2014. The structure is based on, and heavily follows the one proposed by [Noble 2009], with a few but small modifications. The [original repository] has been [modified] by Martin Engqvist and the one presented here differs in some ways. Additional modifictations have been added by Jonas Sindlinger.

[modified]: https://github.com/EngqvistLab/reproducible-research-init
[NESCent]: http://nescent.org
[Noble 2009]: http://dx.doi.org/10.1371/journal.pcbi.1000424
[original repository]: https://github.com/Reproducible-Science-Curriculum/rr-init
