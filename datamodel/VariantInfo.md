# Classification Variant #

Description of entity VariantInfo: variantinfo specific per subject

Attributes:
*	classification: categorical(Clinical Classification (1,2,3,4,5)) - [clinical classification](https://blueprintgenetics.com/variant-classification/)
*	variantID*: string - variantID
*	variant: xref(Variant) - link to variant
*	extra: compound - extra variantInfo
*	gene: string - gene of variant
*	exon: string - exon(s) involved in variant.Format (NM_004006.2:exon3)
*	protein: string - p. notation. Format(NP_003997.1:p.Lys23_Val25del)

---

## Discussion ##


| Attribute | Remarks    | Changed  |
| ---------- | ------------ | ---------- |
