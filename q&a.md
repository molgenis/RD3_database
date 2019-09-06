# Questions & Answers RD3 database


### Dataset
1. Would this be equivalent to an Experiment or rather a cohort? This is, several experiments (WES, WGS, BS-Seq etc. can be done from a single DNA sample). 

**Answer:** Could be cohort, could be experiment. It is a container where files can be linked together. So initially dataset will be experiments, when a subsection of files will be analysed for cohort then datasets can be used as a container with selected files. Moreover it is also a possibility to use more then 1 dataset for cohorts, depends on the need of the user. Therefore it is good idea, when creating datasets, description, type and remarks is filled to see where files where used for.

### Disease
2. We use the Orphanet Rare Disease Ontology (ORDO). In many cases this can be “empty” and inheritance can be filled in.

**Answer:** Now ORDO codes and ICD-10 codes are available. There is no option to fill in inheritance. If there is a new option needed to add other codes, pleas add new issue.

### File
3. File "type" is currently one of "raw data, raw variant, analysis ready", which might be better described as file status. Here I think the "raw data" and "analysis ready" may be useful, but I am not sure about the "raw variant". But in terms of technical type, we currently have 3 - "FastQ" , "BAM" , "gVCF" - for future proofing I would probably add CRAM as well. The FastQs are always compressed of course, but that will be obvious from the filename. I daresay in the future, as a result of analysis output, we will have "VCF"s and "BED"s - for me this would be a more appropriate usage of the file type field.

**Answer:** Type changed to an option field, where choices can be BAM, FastQ, gVCF, CRAM, phenopacket and BED. If more options need to be there in future, those types can be added. To see difference between raw and analysed files best to use Dataset type.

### Job
4. Not sure how this works in practice, because in some cases jobs will be targeting only one experiment and others multiple of them?

**Answer:** Job and run are made to track process of analysis, when everything is working, we need to define which jobs and runs need to be added to the RD3 database. But in theory multiple files can be used as input files and can produce multiple output files, this can be done by one job but can also be done in multiple jobs . And jobs belonging together are joined in a run. But for updating database, need to be decided which jobs are monitored in RD3 database.

### Organisation
5.  Is this the submitting organization of the Solve-RD “experiment”? 

**Answer:** Organisation is now being used for submitting organisation, for example:  cheo-lochmuller and ERN; ERN-NMD. In organisation there is an option to add persons (contactpersons/ investigators, etc) and to add location of organisation. ERN is a text field, so no extra info can be added. 

### Person
6.  Is this to collect the submitter/controller of the files/experiments or anyone that accesses the data? 

**Answer:** Person can be contactperson or principle investigator of an organisation or study. Only people with an account to RD3- database have access to data submitted, these users can be the same as contactperson or principle investigator but don't need to be. 

### Study
7. Unclear how this is implemented in Solve-RD. Is this an experiment for a sample-subject? A cohort? An ERN? Can maybe used in cohorts??

**Answer:** Study can be cohort, or specific part of cohort, or even can be left empty if there is no need to cluster datasets. With study you could link contactpersons, organisation and give a description of study. This could be useful in the future when working with all data from RD3 database. 

### Subject
8. What about prenatal samples? Mother and child?

**Answer:** Can be registered with FID, MID and personal ID

9. It is not entirely clear what happens if a subject has multiple diseases. Is the subject for instance ‘affected’ yes? |

**Answer:** If Yes, then affected main disease codes can be added, otherwise in remarks field can be used to specify for unique situation.

10. In the term ‘variant’ it is not clear if these are variants that the subject is carrying, or if those are variants published in the literature. 

**Answer:** Variants linked to subject are candidate pathogenic variant(s)  

11. The child can have an unknown sex (before analysis)

**Answer:** U, is an option, sex Unknown

### Variant
12. What about structural variations (for instance a translocation?)

Answer: Now not present, only in variantType. Need to know which fields are needed for structural variations, and how it is imported in database.

### Variantinfo
13.  Exon involved in variant. This suggests that the variant includes the exon (as in CNV). Variant located in exon.. (The same location can be different exon numbers, depending on isoform) 

Answer: Exon is string field, when added exon, see format NM_004006.2:exon3, add isoform
