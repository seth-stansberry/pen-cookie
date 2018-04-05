Reproducible Pen Test Reporting
====================

A boilerplate for creating reproducible and consistent note taking structure to put together pen test reports. This project was designed after frustrations with KeepNote and wanting to create a template to keep my reporting more organized through constant note taking. 

Credit
------
> Credit for the original template this was designed around [Cookiecutter Data Science](https://github.com/drivendata/cookiecutter-data-science). The philosophy of [Cookiecutter Data Science](https://github.com/drivendata/cookiecutter-data-science): *A logical, reasonably standardized, but flexible project structure for doing and sharing data science work.*
> Inspiration for this goes to [James Hall](https://411hall.github.io/OSCP-Preparation/) after seeing his template and being impressed. 

Contributing
------------
Pull requests and forks are welcome. This project was designed entirely for my own use for OSCP self study and reporting for CTFs, however anyone else getting milage out of this would be a bonus.

Requirements
------------
Install `cookiecutter` command line: `pip install cookiecutter`    

Usage
-----
To start a new pen test project:

`cookiecutter gh:sethstansberry/cookiecutter-offsec-cookies`

Project Structure
-----------------

```
.
├── AUTHORS.md
├── LICENSE
├── README.md
├── bin                <- Your compiled payloads, scripts can be stored here (not tracked by git)
├── config             <- Configuration files, e.g., for doxygen or for your model if needed
├── data
│   ├── external       <- Data from third party sources.
│   ├── interim        <- Intermediate data that has been transformed.
│   ├── processed      <- The final, canonical data sets for modeling.
│   └── raw            <- The original, immutable data dump.
├── docs               <- Documentation, e.g., doxygen or scientific papers (not tracked by git)
├── notebooks          <- Ipython or R notebooks
├── reports            <- For a manuscript source, e.g., LaTeX, Markdown, etc., or any project reports
│   └── figures        <- Figures for the manuscript or reports
└── src                <- Source code for this project
    ├── data           <- scripts and programs to process data
    ├── external       <- Any external source code, e.g., pull other git projects, or external libraries
    ├── models         <- Source code for your own model
    ├── tools          <- Any helper scripts go here
    └── visualization  <- Scripts for visualisation of your results, e.g., matplotlib, ggplot2 related.
```

Check out my latest research project, which successfully applied the `cookiecutter` philosophy: [SEMIC: an efficient surface energy and mass balance model applied to the Greenland ice sheet](https://gitlab.pik-potsdam.de/krapp/semic-project).

License
-------
This project is licensed under the terms of the [BSD License](/LICENSE)
