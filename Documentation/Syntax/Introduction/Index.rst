.. include:: ../../Includes.txt


.. _syntax-introduction:

Introduction
^^^^^^^^^^^^

TypoScript is internally handled as a (large) multidimensional PHP
array (see ":ref:`what-is-typoscript`"). Values are arranged in a
tree-like hierarchy. The "branches" are indicated with periods
(".") - a syntax borrowed from for example JavaScript and which
conveys the idea of defining objects/properties.


.. _syntax-example:

Example:
""""""""

.. code-block:: typoscript

   myObject = [value 1]
   myObject.myProperty = [value 2]
   myObject.myProperty.firstProperty = [value 3]
   myObject.myProperty.secondProperty = [value 4]

Referring to :code:`myObject` we might call it: "*an object with the value
[value 1] and the property, 'myProperty' with the value [value 2].
Furthermore 'myProperty' has its own two properties, 'firstProperty'
and 'secondProperty' with a value each ([value 3] and [value 4]).*"

The TYPO3 CMS backend contains tools that can be used to visualize the
tree structure of TypoScript. They are described in the relevant
section further in this document (see :ref:`typoscript-templates` and
:ref:`tsconfig`). The above piece of TypoScript would look like this:

.. figure:: ../../Images/SyntaxIntroduction.png
   :alt: Example TypoScript code

