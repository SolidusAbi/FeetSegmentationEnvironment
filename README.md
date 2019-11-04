# FeetSegmentationEnvironment
Anaconda environment used in order to test the code implemented for "Automatic Segmentation based on Deep Learning Techniques fior Diabetic Foot Monitoring through Multimodal Images" (https://doi.org/10.1007/978-3-030-30645-8_38)

# Installation step:
1. Install Anaconda/Miniconda
2. Create a new environment using the "environment.yml" file and activate it
    * conda env create -f environtment.yml -n [Environment Name]
    * conda activate [Environment Name]
3. Build PCL library and install it
    * conda build pcl 
    * conda install file://${CONDA_PREFIX}/conda-bld/linux-64/pcl-1.8.1-0.tar.bz2
4. Build and install python-pcl wrapper
    * conda build python-pcl --python=3.6
    * conda install -c ${CONDA_PREFIX}/conda-bld/ python-pcl
