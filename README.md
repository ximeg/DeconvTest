# DeconvTest: Simulation Framework for Quantifying Errors and Selecting Optimal Parameters of Image Deconvolution

Author: *Anna Medyukhina*

Affiliation: *Research Group Applied Systems Biology - Head: Prof. Dr. Marc Thilo Figge  
https://www.leibniz-hki.de/en/applied-systems-biology.html  
HKI-Center for Systems Biology of Infection  
Leibniz Institute for Natural Product Research and Infection Biology -  
Hans Knöll Insitute (HKI)  
Adolf-Reichwein-Straße 23, 07745 Jena, Germany*

---

DeconvTest is a Python-based simulation framework that allows the user to quantify and compare the
performance of different deconvolution methods. The framework integrates all components needed for such 
quantitative comparison and consists of three main modules: (1) *in silico* microscopy, 
(2) deconvolution, and (3) performance quantification. 

￼<img src="/docs/img/deconvtest_scheme.png" width="600">

## Installation

1. Download [Fiji](https://fiji.sc/#download), make sure that the Fiji installation path does not contain spaces; note the Fiji installation path: you will have to provide it later when installing the DeconvTest packge
1. Download the [DeconvolutionLab_2.jar](http://bigwww.epfl.ch/deconvolution/deconvolutionlab2/) and [Iterative_Deconvolve_3D.class](https://imagej.net/Iterative_Deconvolve_3D) and copy them to the plugins folder of Fiji
1. Install python or [python Anaconda](https://www.anaconda.com/distribution/)
1. Download the [DeconvTest](https://github.com/applied-systems-biology/DeconvTest/releases) package, enter the package directory and install the package by running ``python setup.py install``
1. Provide the path to Fiji when prompted

## Requirements

The software was tested with the following versions of the required packakges:

- scikit-image 0.15.0
- pandas 0.25.1
- numpy 1.16.5
- seaborn 0.9.0
- scipy 1.3.1
- ddt 1.2.1

## License

The source code of this framework is released under the <a href="/LICENSE">3-clause BSD license</a>

## Citation

A. Medyukhina & M.T. Figge (2020) DeconvTest: simulation framework for quantifying errors and selecting optimal parameters of image deconvolution. J. Biophotonics. [https://doi.org/10.1002/jbio.201960079](https://doi.org/10.1002/jbio.201960079)

## Documentation

The DeconvTest package contains several subpackages.

- `classes`: implementation of all classes needed to conveniently work with synthetic image data.
- `modules`: functions to generate synthetic images, deconvolve and quantify the data.
- `batch`: functions to run the framework in a batch mode running multiple processes in parallel.
- `fiji`: ImageJ macros to run the integrated Fiji plugins.
- `scripts`: exemplary scripts and configuration files.
- `tests`: unit tests.

For a detailed user guide, 
see the <a href="https://applied-systems-biology.github.io/DeconvTest/">online documentation</a>

For instructions how to use DeconvTest to optimally deconvolve microscopy images, see the corresponding <a href="https://github.com/applied-systems-biology/DeconvTest/blob/master/docs/DeconvTest_guide_for_microscopy_image_deconvolution.ipynb">jupyter notebook</a>

