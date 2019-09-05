# Subject #

Description of entity Subject: : Human subjects, typically patients or family members

Attributes:

*	FamilyID: string - Family ID (FID)
*	identifier*: string - unique identifier
*	EGA Accession Number: string - EGA Accession Number
*	Claimed sex: xref(Sex) - Claimed Sex / Sex at birth (can be different from observed sex, see sample)
*	variant: mref(Classification Variant) - candidate pathogenic variant(s) for this subject
*	MaternalID: xref(Subject) - Maternal ID (MID)
*	PaternalID: xref(Subject) - Paternal ID (PID)
*	Affected status: bool - whether it is an affected individuals (main disease) Yes/No
*	disease: mref(Disease) - if affected, which MAIN disease code(s) apply to subject
*	phenotype: mref(Phenotype) - Phenotype based on Human Phenotype Ontology (HPO)
*	hasNotPhenotype: mref(Phenotype) - Relevant Phenotype NOT present in subject
*	PhenopacketsID: string - PhenopacketsID
*	Organisation: xref(Organisation) - Name of the organisation that submitted Subject
*	ERN: string - ERN
*	solved: bool - Solved Case for Solve-RD (true/false)
*	Remarks: text - Remarks about this Subject (Relevant for SOLVE-RD project)

---

## Discussion ##


| Attribute | Remarks    | Changed  |
| ---------- | ------------ | ---------- |
| Family relationship | Relations in the PED format | Depended on format PED|
| phenotype | Extra phenotype information by adding:PhenopacketsID? | If needed add new issue |
| Not Present | Cohort building, how do we want to register this? In GPAP or RD3 | Need to be discussed|
