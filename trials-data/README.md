# Trials data

## Tabs

### METADATA
This tab contains a subset of the [Dublin Core Metadata Initiative Terms](https://www.dublincore.org/specifications/dublin-core/dcmi-terms/). `LABEL` and `DEFINITION` provide information about the term, while `VALUE` is the column that should contain your data.
Note that `Title` and `Description` are required fields. These will be used to describe the dataset within Germinate.

### LOCATION
This tab allows you to define (optional) geographic locations that you wish to associate with this dataset. If you wish to provide data from multiple sites, please use a separate copy of this template per location.

### COLLABORATORS
Use this tab to define everyone who should be acknowledged for their contribution to this dataset. Please note that `First Name` and `Last Name` are required fields.

### PHENOTYPES
This is where the traits are defined. Note that only `Name` and `Data Type` are required fields. `Data Type` can only be one of these three options: `int`, `float`, `char`. If unsure, choose `char`. `Short Name` and `Unit Abbreviation` are both limited to 10 characters.

### DATA
This tab is used to define the actual trials data. Germplasm is defined as rows starting from `A2` downwards. Please use the `ACCENUMB` field from the germplasm MCPD standard to identify the material. Traits are defined as columns starting from `D2` to the right. Please use the value from the `Name` column of the `PHENOTYPES` sheet to identify the trait.

The `Rep` and `Treatment` columns are optional. `Rep` can be used if you want to store data for individual replicates. This will create a "Plant/Plot" level entity in Germinate and the data will only indirectly be linked to the germplasm via this "Plant/Plot". You can also opt to use averages across the reps, which you would have to provide. In this case, leave the `Rep` column empty. The `Treatment` column can contain any free-text treatment description that has been applied to this individual.

Please do not remove the `Rep` and `Treatment` columns even if you're not providing any data for them.

The data within each cell can be anything from integers, floating point numbers, text and dates. In the case of dates, we recommend to use the `YYYY-MM-DD` (e.g. 2020-01-02 for January 2nd 2020) date format.

Missing data should be represented by an empty cell (not `NA` or a dash (`-`) or anything else).

### RECORDING_DATES

If you want to associate individual dates with each recording in the `DATA` tab, then please reuse the same structure as in the `DATA` tab, but this time, provide the date of the recording in the cells. These dates have to be in `YYYYMMDD` (e.g. 20200102 for January 2nd 2020) format. If you don't know when the data has been collected, leave this tab as it is.