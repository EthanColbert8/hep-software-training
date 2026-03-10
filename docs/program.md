# Overview of Topics
Welcome! This is an overview of the topics planned (so far) for our "training hackathon".

## Planned Sessions
We're planning to cover these topics as dedicated sessions.

### 1. The Linux Shell: it's all ASCII
A [shell](https://en.wikipedia.org/wiki/Shell_(computing)) is a tool that provides command-driven access to a computer system.
As such, shells are very powerful tools for work and automation.
The [`bash`](https://www.gnu.org/software/bash/) shell (default on most Linux distributions) is the most commonly-seen shell on shared computing resources.
Additionally, numerous conventions exist on Linux systems, which are almost ubiquitous today.
In this session, we will discuss:

1. Using `bash` interactively and basic available commands.
2. Linux-isms: the FHS, installing software, and the [Unix philosophy](https://en.wikipedia.org/wiki/Unix_philosophy).
3. Scripting with `bash`: automation via the shell.
4. (Maybe) Basics of terminal interaction in Windows.

### 2. Git, GitHub, GitLab, and how they're all different
Sharing and co-developing software can quickly get hairy, and software developers almost ubiquitously use [git](https://git-scm.com/docs) and [GitHub](https://github.com/) to help with this.
Additionally, CERN hosts an instance of [GitLab](https://gitlab.cern.ch/), where lots of our shared software lives.
In this session, we will discuss:

1. Using git for version control: what a _repository_ is and why we use them.
2. How git and GitHub (or GitLab, etc.) interact and how code is shared through these services.
3. Collaborating on software projects: git branches, forks, and tags.

### 3. The Purdue Analysis Facility
The [Analysis Facility (AF)](https://analysis-facility.physics.purdue.edu/en/latest/) at Purdue has become one of our most-used platforms for developing and running projects.
In this session, we will discuss:

1. What the AF is, and what happens when you start up an AF server.
2. Managing Python environments on the AF.
3. Overview of the resources available on the AF.

### 4. HPC Clusters and Batch Jobs
Workflows at very large scale are not run interactively, but submitted to large clusters to run in parallel across _many_ CPU cores. In this session, we will discuss:

1. What a _batch scheduler_ is and how they are used to distribute work on large clusters.
2. What a typical batch workflow looks like, in the context of SLURM (and HTCondor?).
3. Connecting to clusters via SSH: SSH keys and configs.
4. The cluster resources available at Purdue (and possibly also lxplus at CERN).

### 5. ROOT
[ROOT](https://root.cern.ch/doc/v636/) is a framework developed by and for HEP scientists doing particle physics analysis.
It is a **very** large library that includes everything and the kitchen sink: four-vector calculations, matrix operations, large dataset handling, statistical fitting, even simplistic MC generation ([`TGenPhaseSpace`](https://root.cern.ch/doc/v636/classTGenPhaseSpace.html)).
As a result, ROOT is very powerful, albeit perhaps less convenient for beginners.
Even outside of ROOT itself, the system ROOT built for serializing (saving) data to files in a compressed, yet easily readable, way is extremely useful, and widely used in HEP even without the ROOT library.
In this session, we will discuss:

1. ROOT files: capabilities and accessing with [Uproot](https://uproot.readthedocs.io/en/latest/).
2. The basics of the ROOT CLI and library.
3. What a ROOT workflow looks like.
4. Using [PyROOT](https://root.cern/manual/python/) to access ROOT functionality in a Python program.

## Extra Materials
These are materials prepared that weren't given a dedicated session, but contain relevant knowledge nonetheless.

### 1. [Python Environments and Development](https://github.com/EthanColbert8/hep-software-training/tree/main/materials/python)
The [Python](https://docs.python.org/3/) language is one of the fundamental tools used today in the scientific community, with numerous libraries developed for general scientific, and HEP-specific, functions.
Creating an _environment_ that contains these tools for your Python code is, unfortunately, far from trivial.
These materials cover:

1. The concept of a _virtual environment_, an important aspect of ensuring Python code runs as expected.
2. The [Conda](https://www.anaconda.com/docs/main) and [Pixi](https://pixi.prefix.dev/latest/) tools for managing virtual environments targeted towards Python execution.
3. Python packages commonly used in HEP, and the wider scientific community.
