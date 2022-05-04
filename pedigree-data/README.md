# Pedigree data

## Tabs

### METADATA
This tab contains a subset of the [Dublin Core Metadata Initiative Terms](https://www.dublincore.org/specifications/dublin-core/dcmi-terms/). `LABEL` and `DEFINITION` provide information about the term, while `VALUE` is the column that should contain your data.
Note that `Title` and `Description` are required fields. These will be used to describe the dataset within Germinate.

Additionally, the fields `Investigation Title`, `Investigation Description`, `Investigation unique ID`, `Associated data file link`, `Associated data file description` and `Associated data file version` are part of [MIAPPE](https://www.miappe.org/).

### ATTRIBUTES
Attributes allow you to define any additional information about the trial. This could be things like irrigation, fertiliser and pesticide information or any other management. Add one "attribute" per row. The type has to be either `numeric`, `date`, `text` or `categorical`.

### COLLABORATORS
Use this tab to define everyone who should be acknowledged for their contribution to this dataset. Please note that `First Name` and `Last Name` are required fields.

### DATA
This tab is used if you know the individuals used to create each germplasm. Please note, that all parents also have to exist in the Germinate database. If you don't want them to be part of the database, please use the `DATA-STRING` tab instead where you can provide the pedigree string in any notation like Lamacraft or Purdy.

Germplasm is defined as rows starting from `A2` downwards. Please use the `ACCENUMB` field from the germplasm MCPD standard to identify the material.
`ACCENUMB`, `Pedigree Description` and at least `Parent 1 ACCENUMB` are required columns. `Parent 2 ACCENUMB` can also be used if known.

### DATA-STRING
Germplasm is defined as rows starting from `A2` downwards. The `Pedigree string` and `Pedigree Notation` columns are required.