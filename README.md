<div align="left">
  <img src="https://github.com/pyscf/pyscf-doc/blob/master/logo/pyscf-logo.png" height="80px"/>
</div>

PySCF documentation
===================

Installation
------------

* Prerequisites
    - [sphinx](https://pypi.org/project/Sphinx/)
    
    - [sphinxcontrib-bibtex](https://pypi.org/project/sphinxcontrib-bibtex/) v1.0.0

    - Set `PYTHONPATH` to include the PySCF source directory; otherwise, uncomment `sys.path.append(os.path.abspath('path_to_pyscf'))` in [source/conf.py](source/conf.py).

* Make HTML pages

        make html

    The resulting html files can be found in the \"build/html\" directory.

How to contribute
-----------------

1.  Add a rst file \"your\_method.rst\" in the [source/user](source/user/) directory in which one describes the basic theory and usage of the method. Reference \"user/your\_method.rst\" in the \"toctree\" section in [source/user.rst](source/user.rst).
2.  Add a rst file \"your\_module.rst\" in the [source/modules](source/modules/) directory in which one lists the examples and the member classes and functions of the module (the API doc is then generated by autodoc). (In the \"\_\_init\_\_.py\" file of each module, one should include a simple usage section. See [pyscf.dft.\_\_init\_\_.py](https://github.com/pyscf/pyscf/blob/master/pyscf/dft/__init__.py) as an example.) Reference \"your\_module.rst\" in the \"toctree\" section in [source/modules.rst](source/modules.rst).
3.  Optionally, one could also add a rst file \"your\_method\_develop.rst\" in the  [source/develop](source/develop/) directory where one provides more detailed descriptions of the implementation and advanced guidelines for using and further development of the module. Reference \"your\_method\_develop.rst\" in [source/develop.rst](source/develop.rst). 
