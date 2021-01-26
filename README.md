# Intelligence and academic performance: Is it all in your head?
To assess how individual variability in psychometric intelligence is associated with student 
performance in an undergraduate physics class, and whether there exists an underlying neural
correlate for such associations, we assessed undergraduate physics students before and after
they took an introductory physics course. A preprint of the manuscript is available on [bioRxiv](https://www.biorxiv.org/content/10.1101/2021.01.23.427928v1),
and the manuscript is currently under review. Here is the code used to run these analyses.
## Code directory
- `gsaw2019/` contains code used in an earlier version of this project, presented at Florida
International University's annual Graduate Student Appreciation Week in 2019 and the following
Florida Council of Graduate Schools Conference.
- `ohbm2019/` contains code used in an earlier version of this project, presented at the annual
meeting of the Organization for Human Brain Mapping in 2019
- `jobs/` contains submission, output, and error scripts for and from running these scripts on 
high-performance computing clusters. It's mostly useless, but included for the sake of transparency.
- `idconn-retrieval/` contains code used to wrangle data, run analyses, and make figures for the manuscript
entitled, *Intelligence and academic performance: Is it all in your head?*, and represents an early
version of the Individual Differences in Connectivity ([IDConn](https://github.com/NBCLab/IDConn)) pipeline.
  1. `preprocessing/` contains code used to preprocess fMRI data, creating participant-specific 
  brain maps, calculating framewise displacement, manipulating confounding variables, etc.
  2. `connectivity/` contains code for computing connectivity matrices from task-based fMRI data
  3. `network-analyses/` contains code for calculating topological measures from these connectivity matrices
  4. `statistics/` contains code for running regressions, ANOVAs, etc. in performing the inferential statistics
  reported in the manuscript
  5. `data-wrangling/` contains code for arranging dataframes to make this all possible
  6. `utils/` contains code for performing quantitative functional decoding of neuroimaging results using
  the [Neurosynth](neurosynth.org) database, ultimately not reported in the manuscript
- `notebooks/` contains Jupyter notebooks used in testing code and making figures seen in the manuscript