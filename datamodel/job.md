# Job #

Description of entity job: jobs used to process sampledata

Attributes:
*	identifier*: string - unique identifier job
*	status: enum - status of job: running, completed or error
*	run*: xref(run) - run this job is part of
*	log: string - uri referencing to logfile
*	inputfile: mref(file) - inputfile, link to file used in job
*	outputfile: mref(file) - file produced with job
*	date: date - date of job
*	jobstart: date - start date and time of job
*	jobend: date - end date and time of job

---

## Discussion ##


| Attribute | Remarks    | Changed  |
| ---------- | ------------ | ---------- |
| Question | Not sure how this works in practice, because in some cases jobs will be targeting only one experiment and others multiple of them | Not Yet |
