.. index::
   single: Forms; Fields; checkbox

checkbox Field Type
===================

Creates a single input checkbox. This should always be used for a field that
has a Boolean value: if the box is checked, the field will be set to true,
if the box is unchecked, the value will be set to false.

+-------------+------------------------------------------------------------------------+
| Rendered as | ``input`` ``checkbox`` field                                           |
+-------------+------------------------------------------------------------------------+
| Options     | - `value`_                                                             |
+-------------+------------------------------------------------------------------------+
| Inherited   | - `data`_                                                              |
| options     | - `required`_                                                          |
|             | - `label`_                                                             |
|             | - `label_attr`_                                                        |
|             | - `read_only`_                                                         |
|             | - `disabled`_                                                          |
|             | - `error_bubbling`_                                                    |
|             | - `error_mapping`_                                                     |
|             | - `mapped`_                                                            |
+-------------+------------------------------------------------------------------------+
| Parent type | :doc:`form </reference/forms/types/form>`                              |
+-------------+------------------------------------------------------------------------+
| Class       | :class:`Symfony\\Component\\Form\\Extension\\Core\\Type\\CheckboxType` |
+-------------+------------------------------------------------------------------------+

Example Usage
-------------

.. code-block:: php

    $builder->add('public', 'checkbox', array(
        'label'     => 'Show this entry publicly?',
        'required'  => false,
    ));

Field Options
-------------

value
~~~~~

**type**: ``mixed`` **default**: ``1``

The value that's actually used as the value for the checkbox. This does
not affect the value that's set on your object.

.. caution::

    To make a checkbox checked by default, set the `data`_ option to ``true``.

Inherited options
-----------------

These options inherit from the :doc:`form </reference/forms/types/form>` type:

.. include:: /reference/forms/types/options/data.rst.inc

.. include:: /reference/forms/types/options/required.rst.inc

.. include:: /reference/forms/types/options/label.rst.inc

.. include:: /reference/forms/types/options/label_attr.rst.inc

.. include:: /reference/forms/types/options/read_only.rst.inc

.. include:: /reference/forms/types/options/disabled.rst.inc

.. include:: /reference/forms/types/options/error_bubbling.rst.inc

.. include:: /reference/forms/types/options/error_mapping.rst.inc

.. include:: /reference/forms/types/options/mapped.rst.inc
