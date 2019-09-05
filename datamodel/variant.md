# variant #

Description of entity variant: variant information according to [HGVS](http://varnomen.hgvs.org/)

Attributes:
*	start_gPosition: int - genomic start position
* hgvs_cdna*: string - hgvs notation for this allele. Format (NM_004006.2:c.4375C>T)
* genomeBuild: categorical(Genome Build) - Human Assembly, genomic build. Format (Mar.2006 (NCBI36/hg18))
*	chromosome: string - chromosome of variant
*	stop_gPosition: int - genomic stop position
*	ref: string - Reference allele
*	alt: string - Alternative allele
* variantType: categorical(Variant Types) - variantType

---

## Discussion ##


| Attribute | Remarks    | Changed  |
| ---------- | ------------ | ---------- |
| Not Present | Missing the ENST or NM number connected to the hgvs_cDNA | part of strin in hgvs_cdna |
| Remark | Variant notation may not work for CNVs (especially ref and alt) | need to add issue, for different format - linked to variantType |
| Not present | option on types of variants other fields visible | Not Yet |
