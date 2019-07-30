# Introduction to Genomic Analysis Workshop Series
> This course is intended for Canadian researchers interested in learning the basic steps of genomic analysis using high performance computing. Using the computing resources of Compute Canada, specifically the WestGrid region, participants will work through practical exercises in the workshop sessions and receive a certificate of completion at the end of the series.  



---
## License
> This work is distributed under the creative commons license (CC BY-SA 3.0).  Details found [here](https://creativecommons.org/licenses/by-sa/3.0/deed.en_US)

## Manuscript
> A manuscript detailing this work can be found here:

[Introduction to Genomic Analysis Workshop: A catalyst for engaging life-science researchers in high throughput analysis](https://f1000research.com/articles/8-1221)

## Downloadable content for adaptable use

The materials are in the process of being re-adapted for the SLURM scheduler, and will be made available via a zenodo link within before the end of 2019. 

## Current workshop materials on Compute Canada Cedar compute cluster

If you are a Canadian researcher, the materials here are present on the Orcinus compute cluster (orcinus.westgrid.ca:/global/scratch/ARC_Training/) and Cedar (cedar.computecanada.ca:/scratch/richmonp/TRAINING/IntroductionToGenomicAnalysis). 


## General Course Information & Prerequisites
### Registering for the course
Please register for the course using our EventBrite Link [here](https://www.eventbrite.ca/e/introduction-to-genomic-analysis-workshop-series-registration-33475860199)

### Course Format

> The course is intended for academic researchers at Canadian institutions in Western Canada, that have access to nationally supported Research Computing through Compute Canada, specifically the WestGrid branch.  

+ 2 hour workshops:
  + 45 minute lecture
  + 15 minute Q&A
  + 45 minute problemset
  + 15 wrap up
+ Each workshop has a prerequisite "quiz".  The problemset from the preceding workshop is the "quiz"
+ If you're familiar with a given subject, you just need to be able to complete the entry quiz instead of attending that subject
  + *Example 1*: Familiar with Linux, but want to learn about short read mapping, do the quiz for Session 2, and show up for Session 3. 
  + *Example 2*: Familiar with short read sequencing analysis and visualization, but want to learn about variant calling, do the quiz for Session 3 and show up to Session 4.
+ Each workshop will have local environment, hosted at BC Children's Hospital with refreshments provided
+ Each workshop will also have a virtual environment, hosted through Vidyo (See details on Vidyo [below](#Software-Installs) )

### Prerequisites  

#### Getting a Compute Canada WestGrid Account  
+ Follow the instructions [here](https://www.computecanada.ca/research-portal/account-management/apply-for-an-account/)
+ If you're a temporary user, refer to the email with instructions to log-in

#### Getting a temporary Compute Canada WestGrid Account  
+ IF YOU ARE UNABLE TO DO THE ABOVE!!!
+ Then a temporary account will be provided to you in the week leading up to the course, and will dissolve when the course completes.

#### Software Installs  
+ Install Vidyo, Instructions [Here](https://github.com/Phillip-a-richmond/Introduction-to-Genomic-Analysis/blob/master/Resources/Vidyo_instructions.md)
+ For mac/linux users, only need native terminal which comes with the operating system.  You can access it in the Applications section for Mac users.  You also need to have X windows installed [Link](https://www.xquartz.org/)
+ For PC users, download and install [MobaXterm](http://mobaxterm.mobatek.net/) 
  + [Advanced MobaXterm usage](https://www.youtube.com/watch?v=Gkl8LD1rwlU)  
+ IGV installed on local machine 
  + [IGV install](https://www.broadinstitute.org/software/igv/log-in) 
+ Filezilla (or other file transfer client) installed on local machine
  + [FileZilla](https://filezilla-project.org/)
  
  ### Resources  
+ [Linux/Unix Cheatsheet](https://github.com/Phillip-a-richmond/ARC-Bioinformatics-Training/blob/master/Resources/UnixCheatSheet.pdf) 
+ [Linux/Unix online tutorial](http://www.ee.surrey.ac.uk/Teaching/Unix/) 
+ Editor cheat sheets 
  + [Emacs cheet sheet](http://www.rgrjr.com/emacs/emacs_cheat.html) 
  + [vi cheat sheet](http://www.lagmonster.org/docs/vi.html) 
  + [nano cheat sheet](http://www.codexpedia.com/text-editor/nano-text-editor-command-cheatsheet/) 
+ File transfer programs  
  + [FileZilla](https://filezilla-project.org/)
  + [WinSCP](https://winscp.net/eng/download.php) 
+ WestGrid resources 
  + [WestGrid website](https://www.westgrid.ca/) 
  + [Running jobs](https://www.westgrid.ca/support/running_jobs) 
  + [Software available](https://www.westgrid.ca/support/software/) 
      
### To-Do before the first class  
1. Get your login information for WestGrid, and log-in to the orcinus compute server.
ssh \<username\>@orcinus.westgrid.ca
example:
ssh richmonp@orcinus.westgrid.ca

2. Complete the Pre-class Quiz found [Here](https://github.com/Phillip-a-richmond/Introduction-to-Genomic-Analysis/blob/master/Assignments/PreQuiz_Session1.txt)

3. Install Vidyo, IGV, FileZilla

---

## Course Details  

### Session 1: Introduction to Linux I, Basic Command Line
> Monday, June 5th, 10:00AM-12:00PM (PST)
+ [Session 1 Pre-Quiz](https://github.com/Phillip-a-richmond/Introduction-to-Genomic-Analysis/blob/master/Assignments/PreQuiz_Session1.txt)
+ [Session 1 Slides](https://docs.google.com/presentation/d/1vaHO9tewJhnpn3CQkIADKnJka4SrKCFb2_zOMTOi7yc/edit#slide=id.g1957375280_1_15)
+ *Linux* 
  + Logging in, filesystem, moving around, file editing, downloading files
  + Commands:
  + cp, ls, mv, cut, mkdir, rm, scp, wget
+ *System tools*: 
  + terminal/shell
+ *Bioinformatics*  
  + File formats: BED, GFF/GTF, VCF
+ [Github Gist](https://gist.github.com/Phillip-a-richmond/8b36d58fb2f03d4760869b0676d50692)
+ [Session 1 Etherpad](https://etherpad.openstack.org/p/Introduction_To_Genomic_Analysis_Session1)
+ [Session 1 ProblemSet](https://github.com/Phillip-a-richmond/Introduction-to-Genomic-Analysis/blob/master/Assignments/Session1_Problemset.txt)
+ [Link to raw recording](https://vidyoreplay.computecanada.ca/replay/showRecordingExternal.html?key=bBtILur7bxNhjMp)
  + Note: Fast-forward to 6:33 for presentation to start
+ [Link to final recording]()


---

### Session 2: Introduction to Linux II, Interacting with the Queue
> Tuesday, June 6th, 10:00AM-12:00PM (PST)
+ [Session 2 Pre-Quiz](https://github.com/Phillip-a-richmond/Introduction-to-Genomic-Analysis/blob/master/Assignments/Session1_Problemset.txt)
+ [Session 2 Slides](https://docs.google.com/presentation/d/1u5R23969caKTCPB3YIYRZRNW2zIcktZJC5S89D-GgjU/edit#slide=id.g1deaa80ad7_0_0)
+ *Linux* 
  + File editor
  + FTP client
  + Shell scripts, interacting with the queue
  + Commands: sh, qsub, qstat, qdel, emacs, 
+ *Bioinformatics* 
  + File formats: FASTQ, FASTQ.GZ 
  + HPC Resources needed: ~1 core/person for 2 hour block  
+ [Github Gist](https://gist.github.com/Phillip-a-richmond/76baff0d4525817e0ca59a638bb374a0)
+ [Session2 Etherpad](https://etherpad.openstack.org/p/Introduction_To_Genomic_Analysis_Session2)
+ [Session 2 ProblemSet](https://github.com/Phillip-a-richmond/Introduction-to-Genomic-Analysis/blob/master/Assignments/Session2_Problemset.txt)
+ [Link to raw recording](https://vidyoreplay.computecanada.ca/replay/showRecordingExternal.html?key=invabc4OKUOtXxa)
  + Note: Fast-forward to 1:52 for presentation to start
+ [Link to final recording]()
  


---

### Session 3: Short read mapping and visualization
> Wednesday, June 7th, 9:30AM-11:30AM (PST)
+ [Session 3 Pre-Quiz](https://github.com/Phillip-a-richmond/Introduction-to-Genomic-Analysis/blob/master/Assignments/Session2_Problemset.txt)
+ [Session 3 Slides](https://docs.google.com/presentation/d/1BJJjY3TaR-TEe8HhBCu1pXp2HFCKgTraRkayrUdvG4Y/edit#slide=id.g1deaa80ad7_0_0)
+ *Bioinformatics*  
  + File formats: SAM, BAM, BAI, sorted.BAM,
  + Tools used: BWA (with different options), samtools, IGV (downloaded on own computer)
  + Datasets: DNA-sequencing (Human)
  + HPC Resources needed: ~4 cores/person for 2 hour block
+ [Github Gist](https://gist.github.com/Phillip-a-richmond/bf669287f33b5bd91c27549b94250834)
+ [Session 3 ProblemSet](https://github.com/Phillip-a-richmond/Introduction-to-Genomic-Analysis/blob/master/Assignments/Session3_Problemset.txt)
+ [Session 3 Etherpad](https://etherpad.openstack.org/p/Introduction_To_Genomic_Analysis_Session3)
+ [Link to raw recording](https://vidyoreplay.computecanada.ca/replay/showRecordingExternal.html?key=ycoB7nogbzccDOO)
  + Note: Fast-forward to 1:28 for presentation to start
+ [Link to final recording]()

---

### Session 4: Variant Calling - Small variants
> Thursday, June 8th, 9:30AM-11:30PM (PST) 
+ [Session 4 Pre-Quiz](https://github.com/Phillip-a-richmond/Introduction-to-Genomic-Analysis/blob/master/Assignments/Session3_Problemset.txt)
+ [Session 4 Slides](https://docs.google.com/presentation/d/1vdX5-nBWnxlQ2C09i8J1OgOwirj-EA-nLwvXOHR58ek/edit#slide=id.g1e4523bd13_1_30)
+ *Bioinformatics*  
  + File formats: VCF
  + Tools used: Picard, GATK, Platypus, Freebayes, Samtools mpileup
  + Datasets: DNA-sequencing (Human)
  + HPC Resources needed: ~4 cores/person for 2 hour block  
+ [Github Gist](https://gist.github.com/Phillip-a-richmond/4f6da08a09881cd088a49d49656ae243)
+ [Session 4 Etherpad](https://etherpad.openstack.org/p/Introduction_To_Genomic_Analysis_Session4)
+ [Session 4 ProblemSet](https://github.com/Phillip-a-richmond/Introduction-to-Genomic-Analysis/blob/master/Assignments/Session4_Problemset.txt)
+ [Link to raw recording](https://vidyoreplay.computecanada.ca/replay/showRecordingExternal.html?key=QJpWP4xxkhLwIyD)
  + Note: Fast-forward to 01:20 for presentation to start
+ [Link to final recording]()

---

### Mid-series Exam
> Friday, June 9th
+ Will be available for answering questions from 10:00-12:00
  + Virtually:  WG_Training room
  + Locally in BCCHR Rm# 2108
+ [Mid-Series Exam](https://github.com/Phillip-a-richmond/Introduction-to-Genomic-Analysis/blob/master/Assignments/Session4_Problemset.txt)
+ [Exam etherpad help](https://etherpad.openstack.org/p/Introduction_To_Genomic_Analysis_Session4)

---

### Session 5: Variant Annotation
> Monday, June 12th, 10:00AM-12:00PM (PST)   
+ [Session 5 Pre-Quiz](https://github.com/Phillip-a-richmond/Introduction-to-Genomic-Analysis/tree/master/Assignments)
+ [Session 5 Slides](https://docs.google.com/presentation/d/1WJ6K-uKoKKcpIA0joufkU4Ym5rF6w3wAahzPWWjHSMs/edit?usp=sharing)
+ *Bioinformatics*
  + File formats: VCF
  + Tools used: GEMINI
  + Datasets: DNA-sequencing (Human)
  + HPC Resources needed: ~4 cores/person for 2 hour block  
+ [Session 5 ProblemSet](https://github.com/Phillip-a-richmond/Introduction-to-Genomic-Analysis/blob/master/Assignments/Session5_Problemset.txt)
+ [Session 5 Etherpad](https://etherpad.openstack.org/p/Introduction_To_Genomic_Analysis_Session5)
+ [Session 5 Github Gist](https://gist.github.com/Phillip-a-richmond/7cce5f287ecc678d29acea980a3086b6)
+ [Link to raw recording](https://vidyoreplay.computecanada.ca/replay/showRecordingExternal.html?key=E2wWUWpLkAZE5aJ)
  + Note: Recording starts at 0:00.


---

### Session 6: RNA-seq I, Read Mapping, Transcript Quantification
> Tuesday, June 13th, 10:00AM-12:00PM (PST) 
+ [Session 6 Pre-Quiz](https://github.com/Phillip-a-richmond/Introduction-to-Genomic-Analysis/blob/master/Assignments/Session4_Problemset.txt)
+ [Session 6 Slides](https://docs.google.com/presentation/d/1QyHtpR6rSRqB_EPY7UuoQY_ufZ8Qp1pctgEQ2hflERs)
+ *Bioinformatics*
  + File formats: GTF review
  + Tools used: HISAT2, stringtie
  + Datasets: RNA-sequencing Inbred Mouse Brain Expression Data
  + HPC Resources needed: ~4 cores/person for 2 hour block 
+ [Session 6 Etherpad](https://etherpad.openstack.org/p/Introduction_To_Genomic_Analysis_Session5)
+ [Session 6 Github Gist](https://gist.github.com/Phillip-a-richmond/ec216db03b1e6c4b1f645934a5c6ebfe)
+ [Session 6 ProblemSet](https://github.com/Phillip-a-richmond/Introduction-to-Genomic-Analysis/blob/master/Assignments/Session6_Problemset.txt)
+ [Link to raw recording](https://vidyoreplay.computecanada.ca/replay/showRecordingExternal.html?key=Bb6vMbJqnF9iwqD)
  + Note: Skip ahead to 00:50 for presentation to start

---

### Session 7: RNA-seq II, Differential Expression
> Wednesday, June 14th, 9:30AM-11:30AM (PST)
+ [Session 7 Pre-Quiz](https://github.com/Phillip-a-richmond/Introduction-to-Genomic-Analysis/blob/master/Assignments/Session6_Problemset.txt)
+ [Session 7 Required Set Up](https://github.com/Phillip-a-richmond/Introduction-to-Genomic-Analysis/blob/master/instructions_deseq_setup.pdf)
+ [Session 7 Slides](https://docs.google.com/presentation/d/1dgLI1qarA3OkFIbIjB0jN2cwjL-jhNqoJumtThw6Fms/edit#slide=id.g1deaa80ad7_0_0)
+ [Session 7 PDF for DESeq](https://github.com/Phillip-a-richmond/Introduction-to-Genomic-Analysis/blob/master/Rtutorial_RNAseq_clustering_DE_ILS_ISS.pdf)
+ [Session 7 R markdown for DESeq](https://github.com/Phillip-a-richmond/Introduction-to-Genomic-Analysis/blob/master/Rtutorial_RNAseq_clustering_DE_ILS_ISS.Rmd)
+ [Session 7 Data Table](https://github.com/Phillip-a-richmond/Introduction-to-Genomic-Analysis/blob/master/ILS_ISS_saline_HTSeq_nostats.txt)
+ [Session 7 Data Covariates](https://github.com/Phillip-a-richmond/Introduction-to-Genomic-Analysis/blob/master/ILS_ISS_saline_HTSeq_nostats_covars.txt)
+ *Bioinformatics*
+ Jasleen Grewal Experience
+ [Link to raw recording](https://vidyoreplay.computecanada.ca/replay/showRecordingExternal.html?key=cbB2f9knXPsiCsZ)
  + Note: Fast-forward to 03:08 for presentation to start


## Example Certificate:
![certificate](https://github.com/Phillip-a-richmond/Introduction-to-Genomic-Analysis/blob/master/Oriol%20Fornés%20Crespo.pdf)


## Proudly Supported By:
+ University of British Columbia Advanced Research Computing
+ BC Children's Hospital Evidence 2 Innovation
+ Compute Canada WestGrid

![BCCH Logo](https://github.com/Phillip-a-richmond/Introduction-to-Genomic-Analysis/blob/master/bcch_logo1.png)

![WestGrid Logo](https://github.com/Phillip-a-richmond/Introduction-to-Genomic-Analysis/blob/master/wesgrid_logo_2016.png)





