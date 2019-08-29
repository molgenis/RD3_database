# variant #

Description of entity variant: identifier of an allele/genotype (HGVS)

Attributes:
*	start_gPosition: int - genomic start position
* hgvs_cdna*: string - hgvs notation for this allele. Format (NM_004006.2:c.4375C>T (Mar.2006: hg18, NCBI36))
*	chromosome: string - chromosome of variant
*	stop_gPosition: int - genomic stop position
*	ref: string - Reference allele
*	alt: string - Alternative allele

---

## Discussion ##


| Attribute | Remarks    | Changed  |
| ---------- | ------------ | ---------- |
| hgvs_cdna | Missing the genome build on which the gPosition is based (for instance GRCh38) | Yes, Added to notation hgvs_cdna|
| Not Present | Missing the ENST or NM number connected to the hgvs_cDNA | Not Yet |
| Not Present | HGVS should be linked to or explained | Not Yet|
| Remark | Variant notation may not work for CNVs (especially ref and alt) | Not Yet |
| Question | What about structural variations (for instance a translocation?) | Not Yet |
| hgvs_cdna | add new option field "human genome reference assembly" | Not Yet |
| Not present | option on types of variants other fields visible | Not Yet |
