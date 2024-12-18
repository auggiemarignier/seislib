.. SeisLib documentation master file, created by
   sphinx-quickstart on Wed Feb 23 14:38:12 2022.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Welcome to SeisLib's documentation!
===================================

``seislib`` is a Python package that allows for obtaining seismic images of the sub-surface from the local to the global scale. It is the result of a long-term effort of our team to make efficient and open source some of the Python codes behind our seismological publications over the last few years. The library is in rapid expansion and, at present, includes:


**Seismic Ambient Noise Interferometry**
	- Automated download of continuous seismograms
	- Fast cross-correlation of continuous seismograms in the frequency domain
	- Extraction of frequency-dependent phase velocities for both Rayleigh and Love waves, based on pairs of receivers
	- Retrieval of frequency-dependent Rayleigh-wave attenuation coefficient, based on dense seismic arrays

**Surface-Wave Tomography based on Teleseismic Earthquakes**
	- Automated download of seismograms recording strong earthquakes
	- Retrieval of frequency-dependent Rayleigh and Love phase velocities, based on pairs of receivers lying on the same great-circle path as the epicentre (Two-Station Method)

**Least-Squares Imaging of Lateral Variations in Surface-Wave Velocity**
	- Equal-area and regular parameterizations, suited for data sets collected at local, regional, and global scale
	- Adaptive parameterizations, with finer resolution in the areas characterized by relatively high density of measurements
	- Linearized inversion of velocity measurements based on ray theory
	- Computational speed optimized (via Cython) for very large data sets
	- Possibility to perform L-curve analyses and resolution tests (e.g., spike, checkerboard)

.. image:: _static/lib_diagram.png
   :align: center

.. warning::

   In the transition from version 0.6.27 to 1.0.0, the `seislib.colormaps` module  was **removed** and replaced by the `cmcrameri` package, which provides the same colormaps previously available in SeisLib.


.. toctree::
   :maxdepth: 1
   :caption: Getting Started
	
   installation
   cite
   
.. toctree::
   :maxdepth: 2
   :caption: Seismic Ambient Noise
   
   seislib.an   

.. toctree::
   :maxdepth: 2
   :caption: Teleseismic Earthquakes
   
   seislib.eq
   
.. toctree::
   :maxdepth: 2
   :caption: Least-squares imaging
   
   seislib.tomography
   
.. toctree::
   :maxdepth: 2
   :caption: Plotting
   
   seislib.plotting

.. toctree::
   :maxdepth: 2
   :caption: Utility Functions
   
   seislib.utils
   

.. toctree::
   :maxdepth: 1
   :caption: Development

   changelog
   licence


