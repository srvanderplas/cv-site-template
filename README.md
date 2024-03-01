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
