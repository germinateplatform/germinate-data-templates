# Image data
Images can be associated with germplasm, traits and chemical compounds. While you can upload images through the Germinate web interface, sometimes it's easier to bulk-upload them using our data templates.

The data template used for image data upload is slightly different from most other templates in that it has to be zipped up (in [ZIP](https://en.wikipedia.org/wiki/ZIP_(file_format)) format) together with the images that should be uploaded. So all you are uploading is a single `.zip` file containing the template file (which HAS to be called `images.xlsx`) and all the images without any subfolders.

The template has 6 columns: `Reference Id`, `Reference Name`, `Image reference type`, `Image filename`, `Image description` and `Tags`, out of which the following are non-optional: `Image reference type`, `Image filename` and EITHER `Reference Id` or `Reference Name`.

Here is an explanation of each column:

- `Reference Id`: The database Reference id of the item you are referencing, e.g. if your `Image reference type` is `germplasm`, then this is the `germinatebase.id`.
- `Reference Name`: Alternatively to the `Id`, the `Reference Name` can be specified. As an example, if you are referencing a `germplasm`, then this has to correspond to the MCPD `ACCENUMB`.
- `Image reference type`: This is one of the following, depending on what the image shows: `germinatebase` (for germplasm), `phenotypes` (for traits) or `compounds`.
- `Image filename`: The file name of the image. This does not include the path, just the filename including the extension, e.g. `P1031523.JPG`.
- `Image description`: An optional description of what the image shows. This can, for example, contain credit information.
- `Tags`: A comma-separated list of tags that should be associated with this image. We recommend using all-lowercase tags with dashes instead of spaces, e.g. `flower` or `whole-plant`.