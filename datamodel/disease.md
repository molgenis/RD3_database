# Disease #

Description of entity disease: ICD-10 codes and Orphanetcodes

Attributes:
*   children: mref(Disease) - link to childeren disease(s)
*   id*: string - Disease code
*   label*: string - name of disease
*   ontology: string - ontology used
*   description: text - description of disease
*   uri: hyperlink - link to more information
*   parentId: xref(Disease) - link to parent disease


---

## Discussion ##


| Attribute | Remarks    | Changed  |
| ---------- | ------------ | ---------- |
| Not present | Should age of onset be included? | This is present in SubjectInfo |
