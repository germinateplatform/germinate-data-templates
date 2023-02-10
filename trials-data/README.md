# Trials data

## Updates

### 2023-02-10

The `Rep` column is now required to contain a value. Even if you're not using reps, please fill the column with something like "1".

### 2021-08-25

The way the `Rep` column is used has changed. Before Germinate would automatically generate Plant/Plot level germplasm for each rep. This will no longer happen. Please fill the column with `1` if you don't have any reps and use the rep number if you do.

## Tabs

### METADATA
This tab contains a subset of the [Dublin Core Metadata Initiative Terms](https://www.dublincore.org/specifications/dublin-core/dcmi-terms/). `LABEL` and `DEFINITION` provide information about the term, while `VALUE` is the column that should contain your data.
Note that `Title` and `Description` are required fields. These will be used to describe the dataset within Germinate.

Additionally, the fields `Investigation Title`, `Investigation Description`, `Investigation unique ID`, `Associated data file link`, `Associated data file description` and `Associated data file version` are part of [MIAPPE](https://www.miappe.org/).

### ATTRIBUTES
Attributes allow you to define any additional information about the trial. This could be things like irrigation, fertiliser and pesticide information or any other management. Add one "attribute" per row. The type has to be either `numeric`, `date`, `text` or `categorical`.

### LOCATION
This tab allows you to define (optional) geographic locations that you wish to associate with this dataset. If the trial has been conducted at different sites, please define them here and reference their `Name` in the `DATA` sheet column `Location`, otherwise leave the `Location` column in the `DATA` sheet empty.

### COLLABORATORS
Use this tab to define everyone who should be acknowledged for their contribution to this dataset. Please note that `First Name` and `Last Name` are required fields.

### PHENOTYPES
This is where the traits are defined. Note that only `Name` and `Data Type` are required fields. `Data Type` can only be one of these four options: `numeric`, `categorical`, `date` and `text`. If unsure, choose `text`. `Short Name` and `Unit Abbreviation` are both limited to 10 characters.

### DATA
This tab is used to define the actual trials data. Germplasm is defined as rows starting from `A2` downwards. Please use the `ACCENUMB` field from the germplasm MCPD standard to identify the material. Traits are defined as columns starting from `D2` to the right. Please use the value from the `Name` column of the `PHENOTYPES` sheet to identify the trait.

The `Block`, `Row`, `Column`, `Treatment` and `Location` columns are optional. `Rep` and `Block` can be used if you want to store data for individual replicates. If you don't have any reps, please fill this column with `1`. `Row` and `Column` can be used to store the location within a trial. The `Treatment` column can contain any free-text treatment description that has been applied to this individual. `Location` indicates the trial site. If this is a multi-site trial, this column is used to indicate which trial a data point originates from. Please declare all locations referenced in this column in the `LOCATION` sheet.

`Latitude`, `Longitude` and `Elevation` on the `DATA` sheet can be used to specify a more detailed location of where the data point has been collected/generated. This information will be used to plot the location of a germplasm within the trial on a map. Please note, that this is different from the locations specified on the `LOCATION` sheet, as these apply to the whole dataset, whereas the `Latitude`, `Longitude` and `Elevation` columns are associated with the data point itself.

Please do not remove the `Rep`, `Block`, `Treatment` or `Location` columns even if you're not providing any data for them.

The data within each cell can be anything from integers, floating point numbers, text and dates. In the case of dates, we recommend to use the `YYYY-MM-DD` (e.g. 2020-01-02 for January 2nd 2020) date format.

Missing data should be represented by an empty cell (not `NA` or a dash (`-`) or anything else).

### RECORDING_DATES

If you want to associate individual dates with each recording in the `DATA` tab, then please reuse the same structure as in the `DATA` tab, but this time, provide the date of the recording in the cells. These dates have to be in `YYYYMMDD` (e.g. 20200102 for January 2nd 2020) format. If you don't know when the data has been collected, leave this tab as it is.