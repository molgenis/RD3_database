# EMX #

The default import format for MOLGENIS is 'EMX'. This is a flexible spreadsheet format (Excel, CSV) that allows you to annotate your data with a data model.

More on how to understand EMX, can be found [here](https://molgenis.gitbooks.io/molgenis/content/guide-emx.html).

## All EMX's present in repo are without data! ##

Datatypes used in RD3 EMX:

| Data type | Expected formatting |
| ------------ | ------------------- |
| string | A string of characters with a length of less than 255 |
| text | A string with characters with a maximum length of 65535 |
| int | Non decimal numbers in range[-2^31 , 2^31 -1] | 
| bool | TRUE/FALSE |
| date | yyyy-mm-dd |
| xref | Id of the attribute you wish to link, this id should always be available in the refEntity. |
| mref | A comma separated list of id’s, these id’s should always be available in the refEntity. |
| categorical | d of the attribute you wish to link, this id should always be available in the refEntity. | 
| hyperlink | A link to a website | 
| email | E-mail adress |
