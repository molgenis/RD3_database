# Dataset #

Description of entity Dataset: collection of files, collected in context of a study. Could also call this a 'fileset' if we like that better

Attributes:
*	description: text - description of the dataset
*	name*: string - name of dataset
*	datafiles: mref(file) - all files in dataset (from 1 run, or all raw datafile with same module, depend on wishes and study

---

## Discussion ##


| Attribute | Remarks    | Changed  |
| ---------- | ------------ | ---------- |
| NO | Would this be equivalent to an Experiment or rather a cohort? This is, several experiments (WES, WGS, BS-Seq etc. can be done from a single DNA sample). | Need to be discussed |
| Not present| Text field for identification incorrect experiment | Not yet |
