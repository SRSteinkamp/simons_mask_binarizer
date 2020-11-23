# simons_mask_binarizer



Not well tested, but should work in most cases. Test of the CLI were only performed on WIN10, so there might be some issues popping up.

Please post an issue, if there is something not working as expected.

## Install

As always I would recommend, creating a new python environment for this tool!

You can then install the package via pip from Github. 
```bash
pip install git+https://github.com/SRSteinkamp/simons_mask_binarizer.git
```

The installation should install all the necessary packages namely (`nilearn` and `nibabel`) and expose the command line tool below. 

## How to use

Currently exposes a CLI directly, to transform single files. In your terminal run:

`nifti_binarizer INPUTPATH -o OUTPUTPATH -p PREFIX`

Where the INPUTPATH (path of the image to be converted) has to be provided.

* `-o` or `--outputpath` argument is optional to provide the destination of the converted image. Defualt image is converted inside `INPUTPATH` folder.

* `-p` or `--prefix` argument is optional, prefix defaults to `bin_`. 

Examples:

```bash
nifti_binarizer C:\some_folder\my_mask.nii.gz` 
```
Creates a new file named as `C:\some_folder\bin_my_mask.nii.gz`. 
```bash
nifti_binarizer C:\some_folder\my_mask.nii.gz -o C:\other_folder\`
```
Creates a new file in `C:\other_folder\bin_my_mask.nii.gz`. 

```bash
nifti_binarizer C:\some_folder\my_mask.nii.gz -o C:\other_folder\ -p 'p'`
```
Creates a new file in `C:\other_folder\pmy_mask.nii.gz`.




