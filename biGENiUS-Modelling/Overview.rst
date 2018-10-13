==================
Modelling Overview
==================

--------------------------------
DWH Objects and DWH Object Types
--------------------------------

DWH Objects
===========
A data warehouse consists of multiple objects: source objects, stage tables, core tables, data mart view. Those objects are represented in biGENiUS by DWH objects.

DWH Object Types
================
DWH objects with same structure and behavior are assigned to the same DWH object type.
A DWH object type is is defined as part of the architecture. How DWH objects may interact with each other is also part of the generator configuration.
The following sections describe the DWH object types used by the MS SQL Server architecture.

DWH Object Types Overview
=========================
.. csv-table:: DWH Object Types Overview
   :header: Type, Source Field Mapping, Data Flow Sources, Relationships to, Has BK, Is Linkable
   :widths: 15 15 15 15 15 15
   
   Stage SQL, Yes, --, --, --, Yes
   Stage composite, --, Stage SQL, --, --, Yes
   Entity, --, Stage SQL /Stage composite, Enity, Yes, Yes
   Fact, --, Stage SQL / Stage composite, Entity, --, Yes
   Mart composite, --, Entity / Fact / Mart composite, --, --, Yes


Some Examples for Boxes, Showing Code and more ...
==================================================

Verschiedene Texthervorhebungen
-------------------------------
Man kann den Text normal, **fett** oder *kursiv* darstellen. Auch ``Schlüsselwörter`` lassen sich 
hervorheben.

Eine numerierte Liste
---------------------
#. Erster Punkt ...
#. Zweiter Punkt ...
#. Dritter Punkt ...

Sourcecode
----------

This is an example code for a term. Also line numbers are shown.

 .. code-block:: sql
    :linenos:

    CASE
       WHEN s1.ListPrice > 500 THEN 'L' 
       WHEN s1.ListPrice > 100 THEN 'M' 
       WHEN s1.ListPrice > 0 THEN 'S' 
       ELSE 'NA' 
    END

Text Boxes (aka Adminitions)
----------------------------

.. caution:: 
    By pressing the ``Return`` key you can save your changes.

.. danger:: 
    By pressing the ``Return`` key you can save your changes.

.. tip:: 
    By pressing the ``Return`` key you can save your changes.

.. note:: 
    By pressing the ``Return`` key you can save your changes.

Hyperlinks
----------

External Links
..............
`Here <https://bigenius.info>`_
you'll find a good resource for more and detailed information.
Direct Link to the biGENiUS Homepage: https://bigenius.info
Some other text ...


Internal Links
..............

You can also work with internal links. Here is a good tutorial 
for doing that: http://www.sphinx-doc.org/en/stable/usage/restructuredtext/roles.html#ref-role


Dimensions
==========

Source systems
==============

Layering
========

