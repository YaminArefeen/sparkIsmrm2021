Example code which runs the experiments for Figure 2, 3, and 4 in the ISMRM abstract "Extending Scan-specific Artifact Reduction in K-space (SPARK) to advanced Encoding and Reconstruction schemes.  requirements.txt contains information about the conda enviorment in which all of these experiments were run.  Due to upload limits, the datasets used in these experiments are not available on github.  Please email yarefeen@mit.edu if you would like access to any of the datasets used for the experiments.  

~~~~~~~~~~~~~~~
sparkFigure2.py
~~~~~~~~~~~~~~~
~Performs SPARK correction to GRAPPA reconstructed kspace from a retrospectively undersampled 3D acquisition.  
~Internal callibration data is used to train both the GRAPPA kernels and the SPARK models
~Utilizes the datasets "kspaceFullFig2.cfl" and "kspaceGrappaFig2.cfl" which can be provided upon request.

~~~~~~~~~~~~~~~
sparkFigure3.py
~~~~~~~~~~~~~~~
~Performs SPARK correction to GRAPPA reconstructed kspace from a retrospectively undersampled 3D acquisition.  
~An external reference is used to reconstruct GRAPPA and reconstruct the undersampled ACS region in the GRAPPA SPARK acquisition.
~Utilizes the datasets "kspaceAcsReconFig3.cfl" and "kspaceGrappaFig3.cfl" which can be provided upon request.


~~~~~~~~~~~~~~~
sparkFigure4.py
~~~~~~~~~~~~~~~
~Simulates SMS and wave-encoded SMS acquisitions and perfomrs the corresponding generalized SENSE reconstruction.
~Applies the SPARK framework to both the cartesian SMS and wave-encoded experiments.
~Utilizes the datasets "kspaceFullFig2.cfl" and "kspaceGrappaFig2.cfl" which can be provided upon request.

