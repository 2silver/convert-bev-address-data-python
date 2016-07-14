The idea for this script is shamelessly copied from https://github.com/BergWerkGIS/convert-bev-address-data

## Why?

The original script only runs on Windows systems. This one performs the same task as the original, but relies on Python.
The gdal Python-Module needs to be installed to perform reprojection.

## Usage

The main difference to the original is that you do not need to specify an input file name. ~~Just execute the script from within the unzipped data from the BEV.~~ The newest version of this script attempts to download the data directly. Of course, you can just put the *.zip file (or its extracted content) in the same directory as the script to avoid an automatic download.

### Command Line Arguments

* The coordinate system of the output file is the WGS84 system by default, but can be specified manually by the -epsg parameter. To produce an output in the Austrian Lambert system, the program call would look like this: `python3 convert-addresses.py -epsg 31287`

* To include the GKZ, use the -gkz parameter 

## License

See https://github.com/scubbx/convert-bev-address-data-python/blob/master/license .
