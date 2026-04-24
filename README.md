<!-- # DAST -->
<h1 align="center"> DAST: DArmstadt Skin Tone Database</h1>
<p align="center">

The DArmstadt Skin Tone (DAST) database contains portrait images from a large variety of capture subjects (light skin to dark skin). Face images are captured under controlled conditions and include ICAO compliant samples as well as systematically overexposed and underexposed images for each subject. In addition, for each subject multiple ground truth measurements for the skin tone are included. The dataset is intended to support the evaluation of demographic bias in face image quality measures and to facilitate the development and benchmarking of skin tone classification.

  <p align="center">
    <a href="https://dasec.h-da.de/staff/christoph-busch/"><strong>Christoph Busch</strong></a>
    ,
    Paul Kibler
    ,
    <a href="https://dasec.h-da.de/staff/fabian-stockhardt/"><strong>Fabian Stockhardt</strong></a>    
    ·
    <a href="https://dasec.h-da.de/staff/christian-rathgeb/"><strong>Christian Rathgeb</strong></a>    

  </p>
  <div align="center">
  </div>

Please contact Christian Rathgeb (christian.rathgeb@h-da.de) or Christoph Busch (christoph.busch@h-da.de) to receive the DAST database.

<p align="center"> 
<img src="12-faces.png" width="50%">
</p>

## Example Data 


    ├───001
    │   ├───Colorimeter
    │   └───Pictures
    │       └───cropped
    ├───002
    │   ├───Colorimeter
    │   └───Pictures
    │       └───cropped
    └───036
        ├───Colorimeter
        └───Pictures
            └───cropped

The images of each subject can be found in the respective subject folder under the subfolder `cropped`. There are 12 .png images per subject: 4 with normal exposure and 8 either underexposed or overexposed. The images were captured using two different cameras.

The exposure level of each image can be determined either from the accompanying CSV file or from the image metadata.

Based on the recording settings, the exposure conditions are defined as follows:

- **1/160 s**: double overexposed (**+2 stops**)
- **1/125 s**: singly overexposed (**+1 stop**)
- **f/11, 1/100 s**: normal exposure (**0 stops**)
- **f/16**: singly underexposed (**−1 stop**)
- **f/22**: double underexposed (**−2 stops**)

This allows the exposure category of each image to be identified directly from its capture parameters.

The colorimeter file is located in the `Colorimeter` subfolder for each subject. 

## Citation 

If you use this work in your publication, please cite the following publications:

```
@inproceedings{Busch-DAST-IWBF-2026,
 Author = {C. Busch and P. Kibler and F. Stockhardt and C. Rathgeb},
 Booktitle = {14th Intl. Workshop on Biometrics and Forensics {IWBF}},
 Publisher = {IEEE},
 Title = {A Skin Tone Annotated Face Image Dataset for Studying Demographic Variability},
 Year = {2026}
}```

