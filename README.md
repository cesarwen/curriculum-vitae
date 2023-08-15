# Cesar Wen Curriculum Vitae

Using lated to create a simple, customizable and modifiable curriculum.

## Table of Contents

- [Cesar Wen Curriculum Vitae](#cesar-wen-curriculum-vitae)
  - [Table of Contents](#table-of-contents)
  - [Introduction](#introduction)
    - [Folder Structure](#folder-structure)
  - [Getting Started](#getting-started)
    - [Prerequisites](#prerequisites)
    - [Installation](#installation)

## Introduction

This project is created to both feature my own curriculum and inspire others to create simple yet effective documents while leveraging and learning latex syntax.

This project is separated in a comprehensive folders inspired by html architecture providing an intuitive structure for both reading and editing.

### Folder Structure

```
├── src                                 # folder containing details latex code to be imported
│   ├── sections                        # foder code for each section of the CV
│   │   ├── work_experience             # foder containing work experience details
│   │   │   ├── giorgio.tex             # description of experience at giorgio
│   │   │   ├── index.tex               # index file for folder, managing other files in it
│   │   │   └── rappi.tex               # description of experience at rappi
│   │   ├── certificate_n_others.tex    # description of certificates and other projects
│   │   ├── education.tex               # description of education
│   │   ├── foreign_languages.tex       # description of foreign languages
│   │   ├── objectives.tex              # description of objectives
│   │   ├── personal.tex                # description of personal data
│   │   ├── skills.tex                  # description of skill sets
│   │   └── summary.tex                 # description of summary section
│   ├── commands.tex                    # custom commands made in latex
│   ├── css.tex                         # custom visual presentation of latex elements
│   └── structure.tex                   # structure order for every section
│── .gitignore
│── main.pdf                            # output pdf file
│── main.tex                            # main file starting the tex program
└── README.md
```

## Getting Started

### Prerequisites

In order to compile this project you will need:
- LaTeX distribution (Xetex or Luatex)
- Fira Sans and Fira Mono as part of system fonts

To edit the output you'll need a text editor such as:
- Visual Studio Code
- TeXstudio
- Notepad ++

### Installation

Here are the steps to compile:

1. Clone this repository
2. Navigate to the project directory through terminal/command line
3. run 
```
xelatex -synctex=1 -interaction=nonstopmode main.tex
```
