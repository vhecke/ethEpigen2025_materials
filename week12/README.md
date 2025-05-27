# Assignment

* Choose a transcription factor (e.g. p300), and obtain peaks from ENCODE (ChIP-seq in a human context!)
* Subset to those peaks that have a predicted distal target(s) using Salviato et al. (2021)
  - You can download a GRanges of those interactions at https://ethz-ins.org/content/hg38.SalviatoDistalEnhancerTargets.GR.rds 
* Label peaks with the genes it is in 3D contact with (henceforth called ‘predicted target(s)’)
* Find the nearest TSS for each peak
* Split the peaks (or genes) into those for which the peak is upstream or downstream of the predicted target
* For each of the two sets, report:
  - 1) in what proportion of the cases the predicted target is the closest gene?
  - 2) plot a distribution of the distances between the peak and the (TSS of the) predicted target gene

Hint:
beware not to count, when calculating proportions, peaks that don’t have interactions with any TSS!

Save your assignment in a R markdown named `assignment.Rmd`, render it, and push the html file to this folder in your github repository
