.. _installation:

====================
Installation
====================

.. currentmodule:: qlib


``Qlib`` Installation
=====================
.. note::

   `Qlib` supports both `Windows` and `Linux`. It's recommended to use `Qlib` in `Linux`. ``Qlib`` supports Python3, which is up to Python3.8.

Users can easily install ``Qlib`` by pip according to the following command:

.. code-block:: bash

   pip install pyqlib


Also, Users can install ``Qlib`` by the source code according to the following steps:

- Enter the root directory of ``Qlib``, in which the file ``setup.py`` exists.
- Then, please execute the following command to install the environment dependencies and install ``Qlib``:
   
   .. code-block:: bash

      $ pip install numpy
      $ pip install --upgrade cython
      $ git clone https://github.com/microsoft/qlib.git && cd qlib
      $ python setup.py install

.. note::
   It's recommended to use anaconda/miniconda to setup the environment. ``Qlib`` needs lightgbm and pytorch packages, use pip to install them.
   


Use the following code to make sure the installation successful:

.. code-block:: python

   >>> import qlib
   >>> qlib.__version__
   <LATEST VERSION>
   
 
You can cd to the qlib/examples to run the example:
 
 .. code-block:: bash
 
      $ qrun benchmarks/LightGBM/workflow_config_lightgbm_Alpha158.yaml
      
.. note::
   If you meet the error like instruments not exists for csi300, you can delete the data and download it again with:
   
   .. code-block:: bash

      $ python scripts/get_data.py qlib_data --target_dir ~/.qlib/qlib_data/cn_data --region cn
      
.. note::
   You may need to install catboost and xgboost before you do run the example.



=====================
