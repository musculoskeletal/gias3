GIAS2 (Geometry Image-Analysis Statistics)
==========================================

A Python library for tools used in musculoskeletal modelling. Includes
tools for parametric meshing, registration, image analysis, statistical
shape modelling, and 3-D visualisation using Mayavi.

Optional dependencies
---------------------

-  VTK and VTK Python bindings (for mesh processing)
-  Mayavi (for 3-D visualisation, requires Numpy, VTK, wxPython,
   configobj)
-  PyCSG (for generating constructive solids)
-  pydicom (for reading DICOM images)
-  Cython (speeds up active shape model and random forest segmentation)
-  matplotlib for some inbuilt plotting functions

Installation
------------

Linux
~~~~~

1. If you would like to use in-built visualisation modules, first
   install Mayavi for you distribution, else you can skip this step.

   1. Install VTK and VTK python bindings (e.g. through your package
      manager). VTK 5.10 is the most stable in my experience with
      Mayavi.
   2. Install mayavi through your package manager (e.g. sudo apt-get
      install mayavi2) or pip (e.g. pip install --user mayavi)

2. Download the
   `wheel <https://bitbucket.org/jangle/gias2/downloads/>`__ and

   ::

       pip install --user [path/to/wheel]

Windows
~~~~~~~

1. The most painless way to install the python dependencies required by
   GIAS2 is to install the umbrella package
   `Anaconda <https://www.continuum.io/downloads>`__.
2. If you would like to use in-built visualisation modules, install
   Mayavi. In you installed Anaconda, from the Anaconda commandline,

   ::

       conda install mayavi

3. Download the wheel and from the Anaconda commandline

   ::

       pip install --user [path/to/wheel]

Examples
--------

Example of some the capabilities of GIAS2 can be found in the
gias2/examples/ directory. We are working to add more examples.

Tutorials
---------

-  `Using GIAS2 with MAP Client for lower limb model
   generation <http://map-client-fai-workshop.readthedocs.io/en/latest/>`__
-  `Using GIAS2 for statistical shape
   modelling <http://gias2-shape-modelling-tutorial.readthedocs.io/en/latest/>`__

License
-------

GIAS2 is under the `Mozilla Public license
2.0 <https://www.mozilla.org/en-US/MPL/2.0/>`__.
