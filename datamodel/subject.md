# Subject #

Description of entity Subject: : Human subjects, typically patients or family members

Attributes:

*	variant: mref(variant) - variant associated to the disease in this subject
*	identifier*: string - unique identifier
*	sex: mref(sex) - sex of the subject
*	clinical_status: enum - whether it is an affected individuals
*	disease: mref(disease) - if affected, which main disease code
*	phenotype: mref(phenotype) - Phenotype based on Human Phenotype Ontology (HPO)
*	hasNotPhenotype: mref(phenotype) - Relevant Phenotype NOT present in subject
*	Organisation: xref(organisation) - Name of the organisation. E.g. University Medical Center Groningen
*	FamilyID: string - Family Number
*	Family entity relationship: categorical(relation) - Family entity relationship

---

## Discussion ##


| Attribute | Remarks    | Changed  |
| ---------- | ------------ | ---------- |
| Family relationship | What about prenatal samples? Mother and child? | added relation |
| Family relationship | Relations in the PED format | Under discussion |
| clinical_status | It is not entirely clear what happens if a subject has multiple diseases. Is the subject for instance‘affected’ yes? | Not Yet |
| variant | In the term ‘variant’ it is not clear if these are variants that the subject is carrying, or if those are variants published in the literature. | Not Yet |
| NOT persent | Subjects table - requires an "ERN" field | Not Yet |
| sex | The child can have an unknown sex (before analysis) | Under discussion |
| phenotype | Extra phenotype information by adding:PhenopacketsID? | Not Yet |
