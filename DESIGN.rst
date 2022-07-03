snfs
====

Abstract Filesystem
-------------------

Interface of files used in this protocol is much abstracted from underlying host system interface, accounting for platform agnositicity
(i.e being able to use it outside of UNIX domain (e.g with NT)).

.. code:: hs

  data Node = File | Folder
  data Folder = [Node]
