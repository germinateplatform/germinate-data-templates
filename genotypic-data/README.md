# Genotypic data

Due to the potentially large data volumes, genotypic data can be provided in two formats. For smaller datasets, we would recommend using the Excel template, while for larger datasets (due to the column number restriction of Excel), you'll have to use the plain text file.
The plain text file is in the same format as the `DATA` tab in the Excel spreadsheet. Additionally, some information from the `METADATA` sheet can be provided as headers.

## Tabs

### METADATA
This tab contains a subset of the [Dublin Core Metadata Initiative Terms](https://www.dublincore.org/specifications/dublin-core/dcmi-terms/). `LABEL` and `DEFINITION` provide information about the term, while `VALUE` is the column that should contain your data.
Note that `Title` and `Description` are required fields. These will be used to describe the dataset within Germinate.

Additionally, the fields `Investigation Title`, `Investigation Description`, `Investigation unique ID`, `Associated data file link`, `Associated data file description` and `Associated data file version` are part of [MIAPPE](https://www.miappe.org/).

`Map Name`, `Marker Technology`, `Genetic or Physical` and `Map Units` are used to create the map within Germinate.

### LOCATION
This tab allows you to define an (optional) geographic location that you wish to associate with this dataset.

### COLLABORATORS
Use this tab to define everyone who should be acknowledged for their contribution to this dataset. Please note that `First Name` and `Last Name` are required fields.

### DATA
This sheet is used to define the actual genotype data. Germplasm is defined as rows starting from `A4` downwards. Please use the `ACCENUMB` field from the germplasm MCPD standard to identify the material. Markers are defined as columns starting from `B3` to the right. Please use the name of the marker as the identifier.

Rows `1` and `2` are used to define an optional map that goes along with the genotypic data. If you're not using a map, leave the rows empty, but don't remove the row identifiers `A1` and `A2`. Linkage groups or chromosomes are defined by their names and the position can be either physical or genetic.

The allele calls are then filled into the cells starting from `B4`. Each cell should contain the allele calls, ideally in the form of two nucleotides for heterozygous data and one for homozygous, e.g. A, T/A, G/C. If the nucleotides aren't known (e.g. only A/B or 0/1 data is available) then this should be provided. Missing data should be represented by an empty cell (not `NA` or a dash (`-`) or anything else).

## Text format
For larger datasets, the format of the `DATA` tab can be reproduced in a plain .txt. file using tab as the delimiter. Please use the following header rows to define the metadata for this dataset:

```
# dataset = Dataset name goes here
# map = Map name here
# markerType = e.g. SNP
```

## Hapmap format
Starting from version 4.2.0, Germinate will support the upload of genotypic data in Hapmap format.