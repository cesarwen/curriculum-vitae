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
├── src
│   ├── sections
│   │   ├── work_experience
│   │   ├── certificate_n_others.tex
│   │   ├── education.tex
│   │   ├── foreign_languages.tex
│   │   ├── objectives.tex
│   │   ├── personal.tex
│   │   ├── skills.tex
│   │   └── summary.tex
│   ├── commands.tex
│   ├── css.tex
│   └── structure.tex
│── .gitignore
│── main.pdf
│── main.tex
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
