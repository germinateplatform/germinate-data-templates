# Chemical Compound data

## Tabs

### METADATA
This tab contains a subset of the [Dublin Core Metadata Initiative Terms](https://www.dublincore.org/specifications/dublin-core/dcmi-terms/). `LABEL` and `DEFINITION` provide information about the term, while `VALUE` is the column that should contain your data.
Note that `Title` and `Description` are required fields. These will be used to describe the dataset within Germinate.

### LOCATION
This tab allows you to define (optional) geographic locations that you wish to associate with this dataset.

### COLLABORATORS
Use this tab to define everyone who should be acknowledged for their contribution to this dataset. Please note that `First Name` and `Last Name` are required fields.

### COMPOUNDS
This is where the chemical compounds are defined. Note that only `Name` is a required fields. `Unit Abbreviation` is limited to 10 characters.

### DATA
This tab is used to define the actual compound data. Germplasm is defined as rows starting from `A2` downwards. Please use the `ACCENUMB` field from the germplasm MCPD standard to identify the material. Compounds are defined as columns starting from `B2` to the right. Please use the value from the `Name` column of the `COMPOUNDS` sheet to identify the compound.

The data within each cells has to be a numeric value.

Missing data should be represented by an empty cell (not `NA` or a dash (`-`) or anything else).

### RECORDING_DATES

If you want to associate individual dates with each recording in the `DATA` tab, then please reuse the same structure as in the `DATA` tab, but this time, provide the date of the recording in the cells. These dates have to be in `YYYYMMDD` (e.g. 20200102 for January 2nd 2020) format. If you don't know when the data has been collected, leave this tab as it is.