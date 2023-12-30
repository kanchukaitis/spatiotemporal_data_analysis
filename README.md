# Spatiotemporal Data Analysis

## Overview
This is a graduate course taught as GEOG696c (the physical geography seminar) at the University of Arizona.  The class was last taught in Fall 2023.  The full syllabus is available [here](https://github.com/kanchukaitis/spatiotemporal_data_analysis/blob/c70773af70425a7ffa5c0f13320f57c5dafd5565/geog696c_syllabus.pdf).

This course is designed as a graduate level class in a workshop format to give students a theoretical framework, practical experience, expert knowledge, and statistical tools for analyzing spatiotemporal datasets. It is fundamentally about [building tools](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2011EO500010) and practical understanding so that students can intelligently apply these techniques in their own research. Topics include basic matrix algebra and statistics, exploratory data analysis, field correlation and regression analysis, autocorrelation and its statistical consequences in time and space, parametric and non-parametric significance testing and error analysis, empirical orthogonal functions including rotation, singular spectrum analysis, maximum covariance and canonical correspondence analysis, and traditional and multitaper spectral analysis.  The course encompasses instruction and training in Python and in the use and manipulation of large multi-dimensional datasets.

The major outcome for the class for each student will be a new and independent analysis of a substantial space-time dataset, a formal manuscript describing the motivation, methods, and results of this analysis, and a professional oral presentation.  Students are encouraged to bring with them or seek out data relevant to their research to use for their final project.  Ideally, students' final projects will provide the material for a thesis chapter and/or peer-reviewed article. 

The course was inspired by and initially based on an objective analysis/spatiotemporal data analysis class taught by [Mike Evans](https://www.geol.umd.edu/~mnevans/).
 
## General Schedule

August 23 to August 31 - [Introduction to Python](https://github.com/kanchukaitis/spatiotemporal_data_analysis/tree/819d6db721c34aa39680e7ff4f72a57fe6611cb9/01_introduction_to_python), [`NumPy`](https://github.com/kanchukaitis/spatiotemporal_data_analysis/blob/main/01_introduction_to_python/introduction_to_numpy.ipynb), [`Pandas`](https://github.com/kanchukaitis/spatiotemporal_data_analysis/blob/main/01_introduction_to_python/introduction_to_pandas_part_1.ipynb), `Matplotlib` ([Part 1](https://github.com/kanchukaitis/spatiotemporal_data_analysis/blob/main/01_introduction_to_python/introduction_to_matplotlib_part_1.ipynb) and [Part2](https://github.com/kanchukaitis/spatiotemporal_data_analysis/blob/main/01_introduction_to_python/introduction_to_matplotlib_part_2.ipynb)) and [Linear Algebra](https://github.com/kanchukaitis/spatiotemporal_data_analysis/tree/main/02_linear_algebra)

August 31 to September 12 - Variance, covariance, and correlation -- [Part 1](https://github.com/kanchukaitis/spatiotemporal_data_analysis/blob/main/03_covariance/covariance_correlation.ipynb) and [Part 2](https://github.com/kanchukaitis/spatiotemporal_data_analysis/blob/main/03_covariance/covariance_correlation_part2.ipynb) -- plus an [introduction to `xarray`](https://github.com/kanchukaitis/spatiotemporal_data_analysis/blob/main/01_introduction_to_python/introduction_to_xarray.ipynb)

September 14 to September 21 - Introduction to Empirical Orthogonal Functions -- [Part 1](https://github.com/kanchukaitis/spatiotemporal_data_analysis/blob/main/04_eofs/eof_with_iris.ipynb) and [Part 2](https://github.com/kanchukaitis/spatiotemporal_data_analysis/blob/main/04_eofs/eof_applied_to_spatiotemporal_field.ipynb) -- plus [mapping with `Matplotlib` and `Cartopy`](https://github.com/kanchukaitis/spatiotemporal_data_analysis/blob/main/01_introduction_to_python/introduction_to_matplotlib_part_2.ipynb) and [singular value decomposition on the covariance matrix vs. the data matrix](https://github.com/kanchukaitis/spatiotemporal_data_analysis/blob/main/04_eofs/eof_covariance_vs_data_matrices.ipynb). 

September 21 to September 28 - [EOF significance](https://github.com/kanchukaitis/spatiotemporal_data_analysis/blob/main/05_significance/eof_significance.ipynb), meaningfulness, and interpretation, with short lectures on [missingness](https://github.com/kanchukaitis/spatiotemporal_data_analysis/blob/main/01_introduction_to_python/missing_data.ipynb) and [randomness](https://github.com/kanchukaitis/spatiotemporal_data_analysis/blob/main/01_introduction_to_python/random_arrays.ipynb).

September 28 to October 10 - EOF interpretation and [orthogonal rotation](https://github.com/kanchukaitis/spatiotemporal_data_analysis/blob/main/06_rotation/eof_rotation_example.ipynb)

October 17 to October 26 - [Analysis of coupled fields](https://github.com/kanchukaitis/spatiotemporal_data_analysis/blob/main/08_mca/mca_example.ipynb), [field correlation](https://github.com/kanchukaitis/spatiotemporal_data_analysis/blob/main/07_correlation_compositing/field_correlation_example.ipynb), an [alternative field correlation approach](https://github.com/kanchukaitis/spatiotemporal_data_analysis/blob/main/07_correlation_compositing/alternative_field_correlation.ipynb) if you need local significance levels, [compositing](https://github.com/kanchukaitis/spatiotemporal_data_analysis/blob/main/07_correlation_compositing/composite_from_list.ipynb), and [field significance and false discovery](https://github.com/kanchukaitis/spatiotemporal_data_analysis/blob/main/09_field_significance/field_significance_false_discovery.ipynb).

October 31 to November 7 - Spectral analysis, [simple periodic signals and auto-correlation](https://github.com/kanchukaitis/spatiotemporal_data_analysis/blob/main/10_spectral/cycles_and_autocorrelation.ipynb), and [singular spectrum analysis](https://github.com/kanchukaitis/spatiotemporal_data_analysis/blob/main/10_spectral/ssa_demonstration.ipynb)

November 9 to November 14 - Frameworks for spatiotemporal data analysis

November 14 to December 5 - Student project work and presentations

## Why Python? 
My own programming career started in FORTRAN and moved to MATLAB, a language I've now spent almost 25 years using effectively and (mostly) without complaint.   But with an increasing number of jobs for earth and environmental sciences student **outside** academia and the rise of Python as the _de facto_ language of data science, I've decided to migrate this class from MATLAB to Python in 2023 (my own research code is also moving, more slowly, in this direction).  This had involved some growing pains (for me!), but in the end I hope that the chance to learn spatiotemporal statistics in a language so widely used across so many fields will be worth the extra trouble for the students who take the class.  For earth scientists relatively new to Python, Martin Trauth's book [Python Recipes for Earth Sciences](https://link.springer.com/book/10.1007/978-3-031-07719-7) provides a useful and broad introduction solidly grounded in the types of analyses many of us are familiar with. 

## Recommended Software Installation 
[This page from DataCamp](https://www.datacamp.com/blog/how-to-install-python) contains useful and straightforward information on getting Python installed on both Windows and Mac.  It provides several options for each but I recommend using Anaconda (e.g. look for the sections with titles 'How to Install Python on Windows Using Anaconda' and 'How to Install Python on macOS Using Anaconda').

[This page from Notable.io](https://noteable.io/jupyter-notebook/install-jupyter-notebook/) also provides simple instructions for getting up and running in Python and Jupyter notebooks. 

[This Youtube video](https://www.youtube.com/watch?v=h1sAzPojKMg&ab_channel=VisualStudioCode) from Visual Studio Code (the integrated coding environment we'll use in this class) can get you up and running pretty quickly. They show installation in Windows, so macOs will be slightly different.  We'll also go this **live** in class on August 24th. 

Here are the basic steps:
* Install Python using Miniconda (recommended for this class: https://docs.conda.io/en/main/miniconda.html) or the full individual Anaconda distribution (https://www.anaconda.com/download) for your operating system.  Both are free.  **Note that if you have an older operating system, the current versions of Miniconda might not work on your system.**  A simple comparison of the benefits and drawbacks of Anaconda vs. Miniconda can be found [here](https://www.earthdatascience.org/workshops/setup-earth-analytics-python/setup-git-bash-conda/).
* From the newly installed Conda prompt, from within Python, or from your terminal, [install iPython](https://ipython.readthedocs.io/en/stable/install/install.html#quick-install).
* Install Juypter Notebooks: https://jupyter.org/install
* Install Visual Studio Code itself (https://code.visualstudio.com/download) for your system
* Within Visual Studio Code, install the Python extensions (from Microsoft)
* Test your system 

## Github

Although not strictly required for this course, I encourage you to use the capacity of Git and Github to streamline your access to and use of the notebooks created for this class, as well as advance your own development of reproducible and readily shareable code.  Here are some good places to start:

* Software Carpentry's [Version Control with Git](https://swcarpentry.github.io/git-novice/)
* Jonathan King's [Github Tutorial](https://jonking93.github.io/Github-Tutorial-Workshop/workshop/welcome). Jonathan took this course as a graduate student. 

## License

This work is licensed under a <a rel="license" href="https://creativecommons.org/licenses/by-nc/3.0/us/">Creative Commons Attribution-NonCommercial 3.0 License (CC BY-NC 3.0 US)</a>. 

You are welcome to use any of this material, so long as it is for non-commercial purposes.

## Resources

This course is designed to open up statistical black boxes and reveal the '[big pile of linear algebra](https://xkcd.com/1838/)' inside.  But of course there are many existing packages that can perform the analyses done in this class and extensions of these in additional dimensions and other applications.  Here are just a few you might find useful:

* [cf-array](https://github.com/xarray-contrib/cf-xarray) - a wrapper for using [CF](https://cfconventions.org/cf-conventions/cf-conventions.html) attributes on xarray objects
* [scikit-learn](https://scikit-learn.org/stable/index.html) - has methods for PCA, CCA, imputation, independent component analysis (ICA), and much much more
* [xeofs](https://github.com/nicrie/xeofs) - being actively developed by Niclas Rieger and as of this writing (November 2023) showing active growth and development of basic EOF methods, multiple field EOF (including MCA), and rotated EOF (see more here: https://xeofs.readthedocs.io/en/latest/) 
* [Pyleoclimate](https://github.com/LinkedEarth/Pyleoclim_util) - extensive package for the analysis of paleoclimate data, including code for the false discovery rate
* [Geopandas](https://geopandas.org/en/stable/) - extends Pandas data types to work with vector geospatial data (including Shapefiles) with operations similar to those available in GIS software
* [fiona](https://fiona.readthedocs.io/en/stable/) - library for reading and writing GIS data formats 
* [rasterio](https://rasterio.readthedocs.io/en/stable/) - read and write to raster data formats like GeoTIFF
* [Xee](https://github.com/google/Xee) - is an Xarray extension for Google Earth Engine 
* [Nitime](https://nipy.org/nitime/index.html) - built for time series analysis in neuroscience, has useful spectral analysis functions like multitaper method
* [multitaper](https://github.com/gaprieto/multitaper) - multitaper spectral methods in Python ([article here](https://doi.org/10.1785/0220210332))
* [mcssa](https://github.com/VSainteuf/mcssa) - univariate Monte Carlo singular spectrum analysis in Python
* [pymssa](https://github.com/kieferk/pymssa) - (multichannel) singular spectrum analysis in Python
* [ecopy](https://ecopy.readthedocs.io/en/latest/ordination.html) - includes methods for PCA, Correspondence Analysis, and ordination
* [GeoCAT](https://geocat.ucar.edu/pages/software.html) - in theory a port of the NCAR Command Language to Python

## Contact

Did you find this course material useful?  Want to share ideas?  Find some bugs? Feel free to contact me at [kanchukaitis@arizona.edu](mailto:kanchukaitis@arizona.edu)
