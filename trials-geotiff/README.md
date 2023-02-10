# Trials geotiffs
Geotiffs are georeferenced images often used to store data raster data in a spatial context. Examples include Unmanned aerial vehicle (UAV)/drone imagery.
Geotiffs can be associated a specific dataset (like a trial) or climate variables/traits.

The data template used for geotiff upload is slightly different from most other templates in that it has to be zipped up (in [ZIP](https://en.wikipedia.org/wiki/ZIP_(file_format)) format) together with the geotiffs that should be uploaded. So all you are uploading is a single `.zip` file containing the template file (which HAS to be called `geotiffs.xlsx`) and all the geotiff images without any subfolders.

The template has 7 columns: `Dataset Id`, `Reference Id`, `Reference Name`, `Image reference type`, `Image filename`, `Image description` and `Recording Date`, out of which the following are non-optional: `Image filename`.

If the geotiff should be associated with a specific dataset (like a trial), please fill the `Dataset Id` column with the id of the dataset and the `Recording Date` column with the date when the geotiff was created in the formay YYYYMMDD (cell must be formatted as 'Text').

If the geotiff should be associated with a specific trait or climate variable, please select the corresponding `Image reference type` and then complete EITHER `Reference Id` OR `Reference Name`.

Here is an explanation of each column:

- `Dataset Id`: The database id of the dataset this geotiff should be associated with.
- `Reference Id`: The database Reference id of the item you are referencing, e.g. if your `Image reference type` is `phenotypes`, then this is the `phenotypes.id` and if  it's `climates`, then this should mirror `climates`.`id`.
- `Reference Name`: Alternatively to the `Id`, the `Reference Name` can be specified. As an example, if you are referencing a `phenotypes`, then this has to correspond to the `Name` column in the trials data template sheet `PHENOTYPES`.
- `Image reference type`: This is one of the following, depending on what the image shows: `climates` (for climate variables) or `phenotypes` (for traits).
- `Image filename`: The file name of the image. This does not include the path, just the filename including the extension, e.g. `GS1_2022-01-01.geotiff`.
- `Image description`: An optional description of what the image shows. This can, for example, contain credit information.
- `Recording Date`: The date at which the geotiff was generated. This has to be specified in the formay YYYYMMDD so 20220103 for the third of January 2022. Please note that the cell has to be of type 'Text'.