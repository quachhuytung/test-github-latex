# Github latex integration
---
## Problem:
1. Lack of version control system(VCS) for document editing, because MS Office(Windows, Mac), Libre Office(Linux) use its own binary files
2. Tex could be a good solution, but it is hard to preview changes in content.
---
## Solution:
- Use Tex with Git to utilize the power of both: Scientific document editing with Tex and Version Control with Git
- Use latexdiff, pdflatex together to generate the difference between two versions.
- Create automated pipeline so that you have to do nothing but wait for it to runs.
---
## How to use this framework:
1. Create a Github Repository with README and .gitignore for Tex([gitignore for latex](https://github.com/github/gitignore/blob/master/TeX.gitignore))
2. Create Github Action in **your new repository** by copying this repository's workflow([workflow](https://github.com/quachhuytung/test-github-latex/blob/master/.github/workflows/blank.yml))
3. Structuring your project **exactly** like this project unless it will not work.  
*You'll need to put your source code in src folder, and the name is main.tex*
4. Push your souce code to Github. Yay, viola. You have nothing to do but wait for the pipeline to run.
---
## Result
### Result by images
### Folder structuring
- src/: Contain your Tex source code
- version/: Contain all the version that have been build, named by Unix timestamp
