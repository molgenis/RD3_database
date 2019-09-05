# Job #

Description of entity job: jobs used to process sampledata

Attributes:
*	identifier*: string - unique identifier job
*	status: enum - status of job: running, completed or error
*	run*: xref(run) - run this job is part of
*	log: string - uri referencing to logfile
*	inputfile: mref(file) - inputfile, link to file used in job
*	outputfile: mref(file) - file produced with job
*	jobstart: date - start date and time of job
*	jobend: date - end date and time of job

---

## Discussion ##


| Attribute | Remarks    | Changed  |
| ---------- | ------------ | ---------- |

