# simons_mask_binarizer



This file will become your README and also the index of your documentation.

## Install

Not yet tested, but should work :)

As always I would recommned, to create a new python environment for this tool!


`pip install git+https://github.com/SRSteinkamp/simons_mask_binarizer.git`

## How to use

Currently exposes a CLI directly, to transform single files. In your terminal run:

`nifti_binarizer INPUTPATH -o OUTPUTPATH -p PREFIX`

Where the INPUTPATH (path of the image to be converted) has to be provided.

The 

* `-o` or `--outputpath` argument is optional to provide the destination of the converted image. Defualt image is converted inside `INPUTPATH` folder.

* `-p` or `--prefix` argument is optional, prefixes to 

