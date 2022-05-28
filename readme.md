# How to analyse LFQ data with R

Most of the script comes directly from the DEP package. For vignette see [link](https://www.bioconductor.org/packages/devel/bioc/vignettes/DEP/inst/doc/DEP.html). In paper/thesis cite [Zhang 2018](https://doi.org/10.1038/nprot.2017.147).

Parts of the script (interactive volcano plots, labeling proteins by function, implementing manual experiment design) were written by Weronika Borek

I debugged and simplified the script and rewritten the second part of it so it is mostly automated (volcanoes based on [Bao et al. 2018](https://elifesciences.org/articles/33465))

Running the script requires additional files: proteinGroups.txt (which you get from MS facility), all_yeast_ORFs.csv (provided) and ExpDesign.csv (example provided). 

You need to modify ExpDesign it to suit your needs in Excel. Label is the variable from "LFQ intensity" column name in proteinGroups. Condition is the new name that you will use in the script. I advise sticking to "a_cond1" etc. syntax, only use alphanumerics and the underscore, and keep it short.

This version was tested only on one set of data. If bugs happen (especially in the second part of script), I will try to address them even when I left the lab (Adele has my email address).

Good luck.   
Ola