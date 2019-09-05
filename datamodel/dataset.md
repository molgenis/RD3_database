# Dataset #

Description of entity Dataset: container of files belonging together (different datasets can contain overlapping files, except for the initial datasets containing start-files (before analysis, start-files = BAM, gVCF files (one per chromosome) and phenopacket file))

Attributes:
*	name*: string - name of dataset
*	description: string - description of the dataset
*	datafiles: mref(File) - all files linked to dataset
*	dataUseConditions: mref(dataUseConditions) - data use conditions for dataset
*	typedataset*: enum - type of dataset (raw or processed (analysed) data)
*	remarks: text - remarks about dataset


---

## Discussion ##


| Attribute | Remarks    | Changed  |
| ---------- | ------------ | ---------- |
| NO | Would this be equivalent to an Experiment or rather a cohort? This is, several experiments (WES, WGS, BS-Seq etc. can be done from a single DNA sample). | See questions |

