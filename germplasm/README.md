# Germplasm MCPD

[Multi-Crop Passport Descriptors](https://www.bioversityinternational.org/e-library/publications/detail/faobioversity-multi-crop-passport-descriptors-v21-mcpd-v21/) is a widely used international standard to facilitate germplasm passport information exchange.

## Tabs

### METADATA
This tab contains a subset of the [Dublin Core Metadata Initiative Terms](https://www.dublincore.org/specifications/dublin-core/dcmi-terms/). `LABEL` and `DEFINITION` provide information about the term, while `VALUE` is the column that should contain your data.
Note that `Title` and `Description` are required fields. These will be used to describe the data resource within Germinate.

Additionally, the fields `Investigation Title`, `Investigation Description`, `Investigation unique ID`, `Associated data file link`, `Associated data file description` and `Associated data file version` are part of [MIAPPE](https://www.miappe.org/).

### DATA
This tab contains all MCPD fields described in the document above. The only required field is `ACCENUMB`, all other fields are optional.
Please check the MCPD standard for data formats and requirements.

Missing data should be represented by an empty cell (not `NA` or a dash (`-`) or anything else).

### ADDITIONAL_ATTRIBUTES
This tab is used to store any kind of information that doesn't fit into the `DATA` sheet. Make sure to use the `ACCENUMB` column from the `DATA` spreadsheet to identify the germplasm and use the column headers for the attribute names. The individual cells then contain the attribute value.

## Example
Have a look at `example-germplasm-mcpd.xlsx` for an example of a completed sheet.