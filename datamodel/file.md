# File #

Description of entity File: individual files on file systems so we can find them back, linked to the datasets describing them.

Attributes:
*	location*: hyperlink - uri referencing file system where this file resides
*	type: enum - Type of file
*	md5: string - hash code to check if file is not corrupted. Discuss: propose to make this required value
*	subject: xref(subject) - PhenoPacket file(s) linked to subject
*	samples: mref(sample) - link to file(s) produced for this sample

---

## Discussion ##


| Attribute | Remarks    | Changed  |
| ---------- | ------------ | ---------- |
| type | Raw and processed data will be in different datasets. | Not Yet |
| type | File "type" is currently one of "raw data, raw variant, analysis ready", which might be better described as file status. Here I think the "raw data" and "analysis ready" may be useful, but I am not sure about the "raw variant". But in terms of technical type, we currently have 3 - "FastQ" , "BAM" , "gVCF" - for future proofing I would probably add CRAM as well. The FastQs are always compressed of course, but that will be obvious from the filename. I daresay in the future, as a result of analysis output, we will have "VCF"s and "BED"s - for me this would be a more appropriate usage of the file type field. | Not yet |
| location | Files organised as /owner/experiment/files internally. | Not Yet |
| Not present | Track the versioning of the files | Not Yet |

