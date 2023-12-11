# IDEAL Lab Project GitHub Template
This template provides a basic file structure for organizing and recording project workflows for various lab research projects.
After cloning a version of this template, your local file system may look something like the following (modified from [JuliaDynamics' Dr. Watson](https://juliadynamics.github.io/DrWatson.jl/dev/) so you may need to modify slightly for Python or other languages as per your specific needs):
```
│projectdir          <- Project's main folder. It is initialized as a Git
│                       repository with a reasonable .gitignore file.
│
├── _notes           <- WIP scripts, code, notes, comments,
│   |                   to-dos and anything in an alpha state.
│   └── tmp          <- Temporary data folder.
│
├── data             <- **Immutable and add-only for project data**
|                       Depending on project this may import repo submodules
│
├── results          <- For outputs needed for reports or papers.
│   |                   
│   └── plots        <- Self explanatory
│   └── videos       <- Can be actual video streams or just gifs/animation files
│   └── tables       <- If helpful to store for papers.
|
├── notebooks        <- Jupyter, Weave or any other mixed media notebooks.
|                       Can reference files in src or utils.
│
├── papers           <- Scientific papers resulting from the project.
|   |                   This will load overleaf links as git submodules.
│   └── reports      <- May also link to report files for sponsor.
|                       
├── scripts          <- Various scripts, e.g. simulations, plotting, analysis,
│                       The scripts use the `src` folder for their base code.
│
├── src              <- Source code for use in this project. Contains functions,
│                       structures and modules that are used throughout
│                       the project and in multiple scripts.
|
├── utils            <- Utility functions brought in from other repos.
|                       May be implemented as submodules if needed (e.g. plotting).
│
├── README.md        <- Optional top-level README for anyone using this project.
├── .gitignore       <- may ignore _notes, data, plots, videos, notebooks,
|                       and latex-compilation related files, etc. as needed
│
├── Manifest.toml    <- Contains full list of exact package versions used currently.
└── Project.toml     <- Main project file, allows activation and installation.
                        Above files can be customized depending on your language
                        Key idea is to make it easy to activate the virtual env
```
