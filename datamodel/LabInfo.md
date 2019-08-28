# LabInfo #
Description of entity LabInfo: information of process in lab (barcodes, sequencer,etc)

Attributes:
*	identifier*: string - sample identifier
*	arrayID: string - arrayID
*	sample: mref(sample) - all sample run in this condition, using same barcode
*	flowcell: string - flowcell information
*	barcode: string - barcode involved
*	samplePosition: string - lane, or possition in well (A1 t/mH12)
*	library: mref(Library) - link to more information about the library used in experiment
*	sequencer: string - sequencerinfo
*	seqType: enum - PE(pair-end), SR (single read)GAP
*	Enrichment kit: string - Enrichment kit

---

## Discussion ##


| Attribute | Remarks    | Changed  |
| ---------- | ------------ | ---------- |
| Remark | We will only be providing some of this information now, but it is great that it is already broader, as this will become more important for new data. | |
| seqType | Different readlengths are possible (for instance SR 35-bp, or PE 150-bp). What about non-Illumina sequencers? Nanopore/PacBio/IonTorrent. Are these supported by this format? | Not Yet |
| Enrichment kit | was caputure kit, changed to enrichment kit | Done |
| Question | Where to put Analysis, metadata? | Answer |
