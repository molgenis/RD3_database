# Sample #

Description of entity Sample: Samples used as input for the analysis

Attributes:
*	identifier*: string - unique identifier
*	alternativeIdentifier: string - alternative identifier used by sample provider
*	ERN: string - ERN
*	anatomicalLocation: xref(AnatomicalLocation)
*	subject: xref(Subject) - reference to the subject from which samples was extracted
*	Claimed sex: xref(Sex) - Claimed Sex / Sex at birth (can be different from observed sex, see sample)
*	Observed sex: xref(Sex) - Computed sex (based on Y- chromosome)
* TissueTypes : xref(TissueTypes) - 
*	materialType: mref(MaterialType) - material type. E.g. DNA
*	QC failed: bool - QC failed (True /False)
* Date available: date - Date that a file became visible to sandbox/RD3
* Sequencing Centre: string - Centre where sample was sequenced
*	organisation: xref(Organisation) - Name of the organisation. E.g. University Medical Center Groningen

---

## Discussion ##


| Attribute | Remarks    | Changed  |
| ------------ | ------------ | ---------- |
|identifier | EGA Accession Number: string - EGA Accession Number| Removed, ONLY for files|
| identifier | persistent identifier (Elixer ID, via SURF) | Need to be discussed |
| Not Present | Samples table requires an "Enrichment kit" | Can be found in Labinfo|
| Not present | “Possible QC fail” and ”Confirmed QC fail” plus text field, need to be added, what about flag boggy samples field?? | Need to be discussed |
