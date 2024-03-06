# Build a Quarto Website off of your CV spreadsheet + bib file

## Requirements:

Files:

- Spreadsheet of talk information    
A starter file is provided in data/CV.xlsx
- bib file of publications    
A starter file is provided in data/CV.bib


Software:

- R
- quarto
- R Packages:
    - magrittr
    - dplyr
    - lubridate
    - stringr
    - purrr
    - RefManageR
    - webshot2

## Layout

- about.qmd - created manually

- talks.qmd - lists anything in posts/talks/*.qmd

- publications.qmd - lists anything in posts/papers/*.qmd

- index.qmd - lists anything in posts/

I have added other folders to my posts/ folder, including `other/`, which is where I put non-automatic posts.

I also have created individual pages on my own site to collect materials for research and teaching. These (at the moment) are manually curated, though it would be fairly easy to build some of the content automatically. 

## Code File Summary

There are 5 code files used to build the project. Only `code/create_posts.R` is intended to be run by the user, and then usually as a pre-build script in `_quarto.yml`.

- `code/common-post-functions.R` contains functions used to build both talks and papers
- `code/image-functions.R` contains functions used to screenshot webpages (used primarily for talks at this point)
- `code/talk-functions.R` contains functions used to build talk posts
- `code/paper-functions.R` contains functions used to build paper posts
- `code/create_posts.R` actually reads in the data in the spreadsheet, 
