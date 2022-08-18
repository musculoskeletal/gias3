GIAS3 (Geometry Image-Analysis Statistics)
==========================================

A Python library for tools used in musculoskeletal modelling. Includes
tools for parametric meshing, registration, image analysis, statistical
shape modelling, and 3-D visualisation using Mayavi.

Modules
-------

This meta-package includes the following modules:

- `gias3.common <https://pypi.org/project/gias3.common/>`_
- `gias3.fieldwork <https://pypi.org/project/gias3.fieldwork/>`_
- `gias3.registration <https://pypi.org/project/gias3.registration/>`_
- `gias3.learning <https://pypi.org/project/gias3.learning/>`_
- `gias3.image-analysis <https://pypi.org/project/gias3.image-analysis/>`_
- `gias3.mesh <https://pypi.org/project/gias3.mesh/>`_
- `gias3.applications (optional) <https://pypi.org/project/gias3.applications/>`_
- `gias3.examples (optional) <https://pypi.org/project/gias3.examples/>`_
- `gias3.io (optional) <https://pypi.org/project/gias3.io/>`_
- `gias3.testing (optional) <https://pypi.org/project/gias3.testing/>`_
- `gias3.visualisation (optional) <https://pypi.org/project/gias3.visualisation/>`_
- `gias3.mapclientpluginutilities (optional) <https://pypi.org/project/gias3.mapclientpluginutilities/>`_
- `gias3.musculoskeletal (optional - requires: OpenSIM) <https://pypi.org/project/gias3.musculoskeletal/>`_

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
-  OpenSIM (required for gias3.musculoskeletal)

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

2. If you would like to use the GIAS3 Musculoskeletal module, you must
   first install OpenSIM to your Python scripting environment. Otherwise,
   you may skip this step. See `Installing OpenSIM`_ for more information.

3. Install GIAS3

   ::

       pip install gias3

Windows
~~~~~~~

1. If you would like to use in-built visualisation modules, first
   install Mayavi, else you can skip this step.

   - If you are using Anaconda to manage your Python environment,
     use conda to install Mayavi (e.g., `conda install mayavi`),
     otherwise, use pip (e.g., `pip install mayavi`).

2. If you would like to use the GIAS3 Musculoskeletal module, you must
   first install OpenSIM to your Python scripting environment. Otherwise,
   you may skip this step. See `Installing OpenSIM`_ for more information.

3. Install GIAS3

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

Installing OpenSIM
~~~~~~~~~~~~~~~~~~

To be able to make use of the GIAS3 Musculoskeletal module, the user must
first install OpenSIM to their Python scripting environment.

First, download OpenSIM from `this <https://simtk.org/frs/?group_id=91>`_ page.

Then, follow the instructions `here <https://simtk-confluence.stanford.edu:8443/display/OpenSim/Scripting+in+Python/#ScriptinginPython-SettingupyourPythonscriptingenvironment>`_
to install OpenSIM to your Python scripting environment.

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
