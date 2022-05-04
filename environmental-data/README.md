# Environmental data

## Tabs

### METADATA
This tab contains a subset of the [Dublin Core Metadata Initiative Terms](https://www.dublincore.org/specifications/dublin-core/dcmi-terms/). `LABEL` and `DEFINITION` provide information about the term, while `VALUE` is the column that should contain your data.
Note that `Title` and `Description` are required fields. These will be used to describe the dataset within Germinate.

Additionally, the fields `Investigation Title`, `Investigation Description`, `Investigation unique ID`, `Associated data file link`, `Associated data file description` and `Associated data file version` are part of [MIAPPE](https://www.miappe.org/).

### ATTRIBUTES
Attributes allow you to define any additional information about the environmental dataset. This could be things like irrigation, fertiliser and pesticide information or any other management. Add one "attribute" per row. The type has to be either `int`, `float` or `char`.

### LOCATION
This tab allows you to define (optional) geographic locations that you wish to associate with this dataset. If you wish to provide data from multiple sites, please use a separate copy of this template per location.

### COLLABORATORS
Use this tab to define everyone who should be acknowledged for their contribution to this dataset. Please note that `First Name` and `Last Name` are required fields.

### ENVIRONMENT VARIABLES
This is where the traits are defined. Note that only `Name` and `Data Type` are required fields. `Data Type` can only be one of these four options: `numeric`, `categorical`, `date` and `text`. If unsure, choose `text`. `Short Name` and `Unit Abbreviation` are both limited to 10 characters.

### DATA
This tab is used to define the actual environmental data. Germplasm is defined as rows starting from `A2` downwards. Please use the `ACCENUMB` field from the germplasm MCPD standard to identify the material. Traits are defined as columns starting from `D2` to the right. Please use the value from the `Name` column of the `ENVIRONMENT VARIABLES` sheet to identify the trait.

The `Date` column describes the date the environmental data has been recorded on. This field is not optional.

The data within each cell can be anything from integers, floating point numbers, text and dates. In the case of dates, we recommend to use the `YYYY-MM-DD` (e.g. 2020-01-02 for January 2nd 2020) date format.

Missing data should be represented by an empty cell (not `NA` or a dash (`-`) or anything else).