DocMaker
========

backup files necessary to create good Latex Docs using LyX

How Does it help:

I have created this repository to backup my work on settings used for
various lyx docs.

    1. Creating a bib style file (.bst).
    Refence in latex files are tricky. I have created takh_JCB.bst

    2. How to use .bst style file in the lyx.
    .bst if the style file for refernce or bibliography. add this bst file to your 
    library. as i have done for mine:

    $sudo cp ./takh_JCB.bst /usr/share/texmf-texlive/bibtex/bst/harvard/
    
    $sudo texhash (update your library)
    
    Now go to lyx and right click on bibligraphy section (at the bottom).Rescan the 
    database of style. Now select your copied bst (takh_JCB).

    3. Removing bordered hyperlink from document citation cross reference.
    Add following to your lyx preamble:
    
    \usepackage{hyperref}
    \hypersetup{colorlinks=true,citecolor=blue}

### Now the crosslinked citation would be in the blue color

