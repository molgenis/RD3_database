# Study #

Description of entity study: container for all activities. Contains datasets

Attributes:
*	study_datasets: mref(dataset) - list of datasets in the study
*	identifier*: string - unique identifier
*	name*: string - human readable label
*	description: text - description of study
*	principleInvestigators: mref(person) - list of investigators responsible
*	organisations: mref(organisation) - list of organisations involved
*	contacts*: mref(person) - list of other contact persons. At least one contact is required
*	website: hyperlink - website of study

---

## Discussion ##


| Attribute | Remarks    | Changed  |
| ---------- | ------------ | ---------- |
| Question | Unclear how this is implemented in Solve-RD. Is this an experiment for a sample-subject? A cohort? An ERN? Can maybe used in cohorts?? | Not Yet |
