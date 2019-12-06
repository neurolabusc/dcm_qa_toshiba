## About

dcm_qa_toshiba is a simple DICOM to NIfTI validator script and dataset to test conversion of [Diffusion Weighted Imaging](https://www.nitrc.org/plugins/mwiki/index.php/dcm2nii:MainPage#Diffusion_Tensor_Imaging) data acquired on Toshiba hardware. Specifically, scientists want gradient vectors to be reported in [FSL format](https://fsl.fmrib.ox.ac.uk/fsl/fslwiki/FDT/FAQ#What_conventions_do_the_bvecs_use.3F) (also described [here](http://justinblaber.org/brief-introduction-to-dwmri/)).

For more details on Toshiba DICOM to NIfTI conversion, see [here](https://github.com/rordenlab/dcm2niix/tree/master/Toshiba).

## 3T Galan Dataset

This dataset was acquired by Clement Debacker using a Toshiba 3T Galan running software V5.0SP6000 courtesy of [ GHU Paris Psychiatrie et Neurosciences](https://www.ghu-paris.fr/en/). Different series were intentionally acquired off-axis to evaluate if gradients are correctly converted to the image-relative coordinates specified by the FSL bvec format.

* Series 6: DTI_SAG_30d
  * On a sagittal view rotation of 30 degrees.

* Series 7: DTI_ortho
  * Axial slices, acquired orthogonal with the scanner bore.

* Series 8: DTI_AX_30d
  * On an axial view rotation of 30 degrees.

* Series 9: DTI_COR_20d
  * On an coronal view rotation of 20 degrees.

* Series 10: DTI_ALL_20d
  * On all view rotation of 20 degrees.

![alt tag](https://github.com/neurolabusc/DistanceFields/blob/master/toshiba.png)