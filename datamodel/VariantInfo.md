# VariantInfo #

Description of entity VariantInfo: extra information about variant

Attributes:
*	protein: string - p. notation
*	name*: string - name of variant
*	variant: xref(variant) - link to variant found in study
*	locus: string - chromosomal locus
*	exon: string - exon involved in variant
*	gene: string - gene of varaiant
*	classification: enum - clinical classification
*	variant_effect: string - variant effect(missense, frameshift, etc.)

---

## Discussion ##


| Attribute | Remarks    | Changed  |
| ---------- | ------------ | ---------- |
| exon | Exon involved in variant. This suggests that the variant includes the exon (as in CNV). Variant located in exon.. (The same location can be different exon numbers, depending on isoform) | Not Yet |
| protein | p-notation needs NP number to identify protein. | Not Yet |
