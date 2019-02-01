
### Construction of canonical model of the dividing human cell
This session will demonstrate various steps needed to construct a canonical model of the dividing human cell in order to integrate the distribution of essential proteins.
We will use a small dataset and go through the following steps:

1. Segmentation of the landmarks (cell and chromosome surfaces) from raw confocal image
* Detection and tracking of chromosome region(s) of interest
* Detection of chromosome segregation
* Detection cell surface
2. Parameters estimation or prediction
* Detection of mitotic stages using chromosome shape
* Prediction of cell division axis using detected chromosome mass
* Extraction of various parameters describing cell and chromosome shape
3. Registration of landmarks
* Registration of chromosome region(s) based on predicted cell division axis
* Registration of cell region based on the predicted cell division axis

4. Representation of cell and chromosome surfaces
* Representation of individual chromosome surface using the cylindrical coordinate system
* Representation of cell surface using cylindrical coordinate system

5. Construction of average landmarks
* Generate average cell and chromosome surfaces in the cylindrical coordinate system
* Convert back to the Cartesian coordinate system 
6. Integrate protein distributions to average landmarks

Afterwards, students will be able work on two additional datasets from different application so that 
they can try to customize the code/ideas to solve different problem(s).

#### Preparation
Students can go through our manuscript below, specially the parts related to construction of canonical model and computation of average protein distributions.
Experimental and computational framework for a dynamic protein atlas of human cell division, Nature 2018
https://www.nature.com/articles/s41586-018-0518-z
 
It would be helpful to visit our project webpage for source code, data, results and the protein atlas, where one can interactively play with different proteins.
http://www.mitocheck.org/mitotic_cell_atlas/

Instruction to use the package is available at https://git.embl.de/grp-ellenberg/mitotic_cell_atlas/blob/master/README.md

#### Important - downloading!!
Complete package containing source code, example and excercise datasets and some precomputed results can be downloaded using 
the following link. Since, this package size is about 5GB, I would recommend participants to download this beofore our session starts.

https://oc.embl.de/index.php/s/6LsFSvHf9c4i4U4

If you face trouble downloading this large file, you can download each part separately using the following 5 links:

Source code:
http://www.mitocheck.org/mitotic_cell_atlas/downloads/v1.0.1/mitotic_cell_atlas_v1.0.1_src.zip

Example dataset
http://www.mitocheck.org/mitotic_cell_atlas/downloads/v1.0.1/mitotic_cell_atlas_v1.0.1_exampledata.zip

Excercise dataset
https://oc.embl.de/index.php/s/AiehCcVtXPmtpMj
 
Since, the entire framework is computationally time damanding even for the example dataset and segmentation of the landmarks is the most time demanding module,
I have created even a smaller dataset by taking few timepoints from each of the cells in example dataset and this minimal dataset could be downloaded using 
the link below:
https://oc.embl.de/index.php/s/kPkCpCYitum34oJ

I have also uploaded segmentation results for entire example dataset that will be used for constructing the canonical model. It could be downloaded
using the link below:  
https://oc.embl.de/index.php/s/nInhhq328e1Wlcs
 
#### Requirements
A MATLAB installation with the following toolboxes is required:

* Statistics and Machine Learning Toolbox
* Image Processing Toolbox
* Curve Fitting Toolbox
* Computer Vision System Toolbox 

All students are requested to make sure that they have access to MATLAB by Feb 2nd, so that we are ready for next day. 
