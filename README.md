# Waro Map Tool

This repository contains the source files for Motu's online tool for mapping Māori-owned land in the East Cape.

The tool was created by [Sam Liberman](https://motu.nz/about-us/people/sam-liberman/) for [the Waro project](https://waro.nz/).
Its intended use is for Māori landowners to visualise land eligibility for the New Zealand Emissions Trading Scheme (ETS) and for the Gisborne district’s Erosion Control Funding Programme (ECFP).

The geoprocesing was done using [ESRI ArcMap 10.6](http://desktop.arcgis.com/en/arcmap/).
The Māori Land Court data was clipped first to the Gisbourne district and then to a historical LUC land layer of forest in 1990 to determine which Māori land would be ETS eligible.
Then, a current LUC layer was used to clip the ETS eligible layer to determine which areas are classified as 6e, 7e and 8e land.
This produced the ECFP eligible layer.
The Māori Land Blocks layer, the ETS eligible layer, and both the ETS and the ECFP eligible layer were transferred to [QGIS](https://www.qgis.org/en/site/), where they were exported to an interactive web version using [the qgis2web plugin](https://github.com/tomchadwin/qgis2web).

## Usage

The map can be viewed [here](https://moturesearch.github.io/waro-map-tool).
It can also be downloaded for offline use by creating a local copy of this repository and opening `index.html`.

## License

All repository contents are licensed under the [MIT license](https://github.com/moturesearch/waro-map-tool/blob/master/LICENSE).

