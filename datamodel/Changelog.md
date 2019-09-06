# ChangeLog
All notable changes to this project will be documented in this file.

## [1.1] - 2019-09-06
  
During weekly meetings there were needs expressed for new fields or options. These requested were gather and were updated in new datamodel. Version 1 was Draft model, without any input from Solve-RD project.
 
### Added

All ontolology codelist were filled:
* anatomicalLocation: SNOMED CT
* Disease: ICD-10 codes and ORDO codes
* materialType: MIABIS code list 
* phenotype: HPO code list
* sex: MIABIS code list 
* GenomeBuild: UCSC options
----
New Entities were added:
* GenomeBuild
* Filetype
* ClinicalClassification
* VariantTypes
* SequencingTechniqueType
----
Per Entity attributes that are added:

| Entity | Attribute |
| ------ | ------ |
| Dataset | remarks |
| Dataset | typedataset |
| File | EGA Accession Number |
| File | Flag Abnormal File |
| Sample | EGA Accession Number |
| Sample | ERN |
| Sample | Flag Abnormal |
| Sample | Claimed sex |
| Sample | Observed sex |
| Subject | EGA Accession Number |
| Subject | ERN |
| Sample | FamilyID |
| Sample | Paternal ID |
| Sample | Maternal ID |
| Sample | Solved |
| Sample | Remarks |
| SubjectInfo | Date of birth |
| SubjectInfo | ageOfOnset |
| SubjectInfo | ageOfDiagnosis |
| Variant | genomeBuild |
| VariantInfo | Description |



 
### Removed
Per Entity attributes that are removed:

| Entity | Attribute | Reason |
| ------ | ------ | ------|
| Library | libraryStrategyId | sequencing technique already in Labinfo; seqType |
| Library |  librarySourceId | type of source material already in Sample: materialType |
| disease inheritance | all | for now not specified |
| Job | Date | lready start and stop date present |
| relation | all | Not needed FID/MID/PID added |
| SubjectInfo | comments | already present in Subject |


### Other

| Entity | Attribute | What? |
| ---- | ----- | ------ |
| Labinfo | seqType | extra options added, for non-Illumina sequencers and SR 35-bp, or PE 150-bp |
| Labinfo  | caputure kit | name changed to enrichment kit |
| sex | label | option added UD; undifferentiated, the gender could not be uniquely identified such as hermaphrodite |
| VariantInfo | name | attribute name variantInfo changed to Classification Variant (specificly linked to subject, variant is technical information on variant) |

 

 
