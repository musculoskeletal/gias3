GIAS3 (Geometry Image-Analysis Statistics)
==========================================

A Python library for tools used in musculoskeletal modelling. Includes
tools for parametric meshing, registration, image analysis, statistical
shape modelling, and 3-D visualisation using Mayavi.

Modules
-------

This meta-package includes the following modules:

- gias3.common
- gias3.fieldwork
- gias3.registration
- gias3.learning
- gias3.image-analysis
- gias3.mesh
- gias3.applications (optional)
- gias3.examples (optional)
- gias3.io (optional)
- gias3.testing (optional)
- gias3.visualisation (optional)
- gias3.mapclientpluginutilities (optional)
- gias3.musculoskeletal (optional - requires: OpenSIM)

See `Installing optional modules`_ for more information.

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
   install Mayavi for your distribution, else you can skip this step.

   1. Install VTK and VTK python bindings (e.g., through your package
      manager). VTK 5.10 is the most stable in my experience with
      Mayavi.
   2. Install mayavi through your package manager (e.g. `sudo apt-get
      install mayavi2`) or pip (e.g., `pip install --user mayavi`)

2. Install GIAS3

   ::

       pip install gias3

Windows
~~~~~~~

1. If you would like to use in-built visualisation modules, first
   install Mayavi, else you can skip this step.

   - If you are using Anaconda to manage your Python environment,
     use conda to install Mayavi (e.g., `conda install mayavi`),
     otherwise, use pip (e.g., `pip install mayavi`).

2. Install GIAS3

   ::

       pip install gias3

Installing optional modules
~~~~~~~~~~~~~~~~~~~~~~~~~~~

Optional GIAS3 modules can be included in the installation by passing the
corresponding keywords to `pip`:

- `apps` = gias3.applications
- `examples` = gias3.examples
- `tests` = gias3.testing
- `vis` = gias3.visualisation
- `io` = gias3.io
- `mapclient` = gias3.mapclientpluginutilities
- `musculoskeletal` = gias3.musculoskeletal

For example, if you want to include the modules `gias3.applications` and
`gias3.visualisation` in addition to the default modules, use the command,

::

   pip install gias3[apps,vis]

Tutorials
---------

-  `Using GIAS3 with MAP Client for lower limb model
   generation <http://map-client-fai-workshop.readthedocs.io/en/latest/>`__
-  `Using GIAS3 for statistical shape
   modelling <http://gias3-shape-modelling-tutorial.readthedocs.io/en/latest/>`__

License
-------

GIAS3 is under the `Mozilla Public license
2.0 <https://www.mozilla.org/en-US/MPL/2.0/>`__.
