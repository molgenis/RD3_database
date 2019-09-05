# LabInfo #
Description of entity LabInfo: information of process in lab (barcodes, sequencer,etc) linked to sample(s)

Attributes:
*	identifier*: string - sample identifier
*	arrayID: string - arrayID
*	sample: mref(sample) - all sample run in this condition, using same barcode
*	flowcell: string - flowcell information
*	barcode: string - barcode involved
*	samplePosition: string - lane, or possition in well (A1 t/mH12)
*	library: mref(Library) - link to more information about the library used in experiment
*	sequencer: string - sequencerinfo
*	seqType: xref(SequencingTechniqueType) - sequencing technique types (e.g. WXS, WGS)
*	Enrichment kit: string - Enrichment kit

---

## Discussion ##


| Attribute | Remarks    | Changed  |
| ---------- | ------------ | ---------- |
| Remark | We will only be providing some of this information now, but it is great that it is already broader, as this will become more important for new data. | |
| Question | Where to put Analysis, metadata? |If extra fields are necessary, add new issue|
