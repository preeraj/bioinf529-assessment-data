# bioinf529-assessment-data
This repo contains the data that will be used in your placement assessment.
Therefore, the description of the data is as follows:

---
## Description

The data contains four (4) columns:

|#|Column|Description|
|:--|:--|:--|
|1|`start`| the starting position of a region|
|2|`end`| the ending position of a region|
|3|`seq`| the reference sequence of the region|
|4|`info`| whether or not the region has an observed variation|

The `info` column is the most crucial part of a given row. If no
variant was found within the row's regions of interest, the column 
will have `No_variant` as its contents. However, if a variant is 
found in the region of interest, the contents will be *similar* to 
> `Variant_<some_number>_<some_letter(s)>`

This means that at that position (`<some_number>`) within the region
of interest, a variant (`<some_letter(s)>`) was found that is different
than the original sequence (the sequence found in the `seq` column).