# disease inheritance #

Description of entity disease inheritance : description of known inheritance linked to disease and possibly mutation

Attributes:
*	disease: mref(disease) - disease linked to this inheritancemode
*	identifier*: string - unique identifier
*	variant: mref(variant) - variant link to this inheritancemode
*	inheritancemode: enum - can be categorical, WT, x-linked, recessive, dominant, (als het om syndroom gaat, dan zie je dit ook in disease (orphanet))


---

## Discussion ##


| Attribute | Remarks    | Changed  |
| ---------- | ------------ | ---------- |
| ALL | We don’t use the inheritance linked to a disease (it’s independent), as it is based on the family history mainly. | Not yet |
| ALL | we use HPO to code for it. In many cases “inheritance” is filled in but “disease” is empty | Not Yet |
| inheritancemode | It is better to write out WT in full and I would say X-linked | Not Yet |
