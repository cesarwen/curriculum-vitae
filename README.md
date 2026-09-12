# Cesar Wen Curriculum Vitae Template
Crafting Simplicity, Customizability, and Flexibility with LaTeX
## Table of Contents

- [Cesar Wen Curriculum Vitae Template](#cesar-wen-curriculum-vitae-template)
  - [Table of Contents](#table-of-contents)
  - [Introduction:](#introduction)
    - [Folder Structure](#folder-structure)
  - [Getting Started](#getting-started)
    - [Prerequisites:](#prerequisites)
    - [Installation](#installation)

## Introduction:

This endeavor aims to showcase my personal curriculum vitae while also serving as an inspiration for individuals seeking to fashion straightforward and impactful documents through the utilization and comprehension of LaTeX syntax.

The project is meticulously organized into distinct folders, drawing inspiration from HTML architecture. This approach ensures an intuitive framework for seamless navigation, reading, and editing, enhancing both user experience and document management.

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
│   │   ├── personal.tex                # description of personal data
│   │   └── skills.tex                  # description of skill sets
│   ├── commands.tex                    # custom commands made in latex
│   ├── css.tex                         # custom visual presentation of latex elements
│   └── structure.tex                   # structure order for every section
│── .gitignore
│── main.pdf                            # output pdf file
│── main.tex                            # main file starting the tex program
└── README.md
```

## Getting Started

### Prerequisites:

Before compiling this project, ensure that you have the following prerequisites in place:

- A LaTeX distribution (XeTeX or LuaTeX) installed on your system.
- Fira Sans and Fira Mono fonts available as part of your system's font collection.

For editing the output, you will need a text editor. Some recommended options include:

- Visual Studio Code
- TeXstudio
- Notepad ++

### Installation

To successfully compile the project, follow these steps:

- Clone this repository to your local machine.
- Using your terminal or command line, navigate to the project directory.
- Execute the following command to initiate the compilation process:

```
xelatex -synctex=1 -interaction=nonstopmode main.tex
```

By following these steps, you'll be able to compile the LaTeX project successfully and generate the desired output.

## Automated PDF builds

The [Build CV PDF workflow](.github/workflows/build-cv.yml) compiles `main.tex`
with XeLaTeX whenever a pull request is merged into `main` (or a commit is pushed
directly to `main`). It uses the full TeX Live environment and registers the Fira
fonts required by the CV.

To build manually, open **Actions → Build CV PDF → Run workflow**, select `main`,
and click **Run workflow**. The manual trigger becomes available once this workflow
is on the repository's default branch.

Download the PDF from **Actions → Build CV PDF → a successful run → Artifacts**.
The filename follows `cvCesarWen<BranchName>.pdf`, so builds on `main` produce
`cvCesarWenmain.pdf`. Artifacts are retained for 90 days, subject to repository
retention limits. No additional secrets or release setup are required.
