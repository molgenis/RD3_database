# File #

Description of entity File:  individual files on file systems, files are linked in datasets, versioning with EGA accession number.

Attributes:
* EGA Accession Number: string - EGA Accession Number
* location*: hyperlink - uri referencing file system where this file resides
* md5: string - hash code to check if file is not corrupted. Discuss: propose to make this required value
* typeFile: categorical(File type) - type of file (BAM, FastQ, gVCF, phenopacket, BED, etc.)
* samples: mref(Sample) - link to file(s) produced for this sample
* Flag Abnormal File: bool - flag abonormal file (True /False)

---

## Discussion ##


| Attribute | Remarks    | Changed  |
| ---------- | ------------ | ---------- |
| type | Raw and processed data will be in different datasets. | See dataset |
| location | Files organised as /owner/experiment/files internally. | Need to be imported from sandbox |
| Not present | Track the versioning of the files | Need discussion, maybe with EGA Accession Number|

