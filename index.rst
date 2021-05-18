.. OpenSeesPy documentation master file, created by
   sphinx-quickstart on Tue Sep 26 12:56:27 2017.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

.. include:: src/sub.txt

.. important::

   此版本非官方版本，此版本为笔者对原文的中文翻译版。仅用于学习交流。
   
   由于笔者语言水平有限，翻译可能存在一定偏差，在难以理解的部分可寻找原文档进行深入探究。

   本文正处于翻译过程中，因此会显示为中英文混合在一起的状态。

   Version |opspy_version| is released!

   OpenSeesPy is on :doc:`src/pypi`.

   The latest version of this document can be found at
   `<https://openseespydoc.readthedocs.io/en/latest/>`_.

.. note::

   Questions including modeling issues and the use of OpenSeesPy,
   please post on `OpenSeesPy Forum <https://opensees.berkeley.edu/community/viewforum.php?f=12>`_.

   You are very welcome to contribute to OpenSeesPy with new command
   documents and examples
   by sending pull requests
   through `github pulls <https://github.com/zhuminjie/OpenSeesPyDoc/pulls>`_.

   For errors in this document, submit on 
   `github issues <https://github.com/zhuminjie/OpenSeesPyDoc/issues>`_.


========================
  OpenSeesPy 库
========================

`OpenSeesPy`是采用 `Python 3`解释的 `OpenSees`_.
以下是一个最简单的代码:

::

   # import OpenSeesPy
   import openseespy.opensees as ops

   # import OpenSeesPy plotting commands
   import openseespy.postprocessing.Get_Rendering as opsplt

   # wipe model
   ops.wipe()

   # create model
   ops.model('basic', '-ndm', 2, '-ndf', 3)

   # plot model
   opsplt.plot_model()

To run a test of the pip installation:

::

   pytest --pyargs openseespy.test


============
 Developer
============
原作者：
*Minjie Zhu*

| Research Associate 
| Civil and Construction Engineering
| Oregon State University

翻译：
*Li Zhengning*

   
.. toctree::
   :maxdepth: 1
   :numbered:
   :caption: Contents
      
   src/installation
   src/compile
   src/changelog
   src/modelcmds
   src/analysiscmds
   src/outputcmds
   src/utilitycmds
   src/fsicmds
   src/senscmds
   src/reliabilitycmds
   src/parallelcmds
   src/preprocessing
   src/postprocessing
   src/examples


   

.. raw:: html

   <script type='text/javascript' id='clustrmaps' src='//cdn.clustrmaps.com/map_v2.js?cl=ffffff&w=70&t=n&d=SKQBbxa32RopNU9415W5PDNgdO0XjXnxv2wJdeH0CHw'></script>
