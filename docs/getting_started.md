# Getting started

## Using `cookiecutter`

1. Install `cookiecutter`: `pip install cookiecutter`    
2. Use template `cookiecutter gl:martisak/paper-template`.
~~~~
full_name [John Smith]:
email [john.smith@cyberdyne.com]:
affiliation [Cyberdyne Systems]:
department [Special Projects]:
paper_title [Name of your paper]:
paper_slug [name-of-your-paper]:
paper_short_description [A short description of your paper]:
release_date [2019-02-16]:
Select template:
1 - NeurIPS
2 - ICML
3 - ACM CCS
4 - IEEE
5 - KTH Master Thesis
6 - Generic article
Choose from 1, 2, 3, 4, 5, 6 (1, 2, 3, 4, 5, 6) [1]: 3
~~~~

3. Edit your document.
4. Run `make` to compile the document.
5. If you are using Gitlab CI, pushing this example will create an artifact.

### Document metadata

The document metadata is slightly different depending on the template, even though we strive to align the different templates.

~~~~
---
title: Paper template
author:
    - name: Your name here
      email: your_name@domain.com
      affiliation: 1  
    - name: Miles Dyson
      email: miles@cyberdynesystems.com
      affiliation: 1 
affiliation: 
  - Cyberdyne Systems
keywords: open science, reproducible research, literate programming
abstract: |
  Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
  tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
  quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
  consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
  cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
  proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
---
~~~~

### Document body

The document body can contain Markdown or LaTeX code.

### Code

You can optionally include chunks of R code (via Knitr) or Python code (via pweave). Knitr also supports a lot of other languages.
