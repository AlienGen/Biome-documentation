.. orm:

ORM
***

Model definition
================

Object structure
----------------

Field
-----

PrimaryField
^^^^^^^^^^^^

TextField
^^^^^^^^^

PasswordField
^^^^^^^^^^^^^

TextAreaField
^^^^^^^^^^^^^

BooleanField
^^^^^^^^^^^^

DoubleField
^^^^^^^^^^^

DateField
^^^^^^^^^

TimeField
^^^^^^^^^

DateTimeField
^^^^^^^^^^^^^

EnumField
^^^^^^^^^

Many2OneField
^^^^^^^^^^^^^

One2ManyField
^^^^^^^^^^^^^

Many2ManyField
^^^^^^^^^^^^^^

Function
--------

Basic operations on model
=========================

Retrieve
--------

.. code-block:: php

	<?php

	/* Retrieve all the objects. */
	MyModel::all();

	/* Retrieve the object of id 10, throw an exception if not found. */
	MyModel::get(10);

	/* Retrieve the object of id 10, return null if not found. */>
	MyModel::all()->filter('id', '=', 10)->current();

Creation
--------

.. code-block:: php

	<?php

	/* Create an instance of MyModel. */
	$object = new MyModel();

	/* Define the value of the attributes. */
	$object->name = "My name";

	/* Save the object. */
	$object->save();

Update
------

.. code-block:: php

	<?php

	/* Get the object of id 10. */
	$object = MyModel::get(10);

	/* Define the value of the attributes. */
	$object->name = "My object of id 10";

	/* Save the object. */
	$object->save();

Delete
------

.. code-block:: php

	<?php

	/* Get the object of id 10. */
	$object = MyModel::get(10);

	/* Delete the object of id 10. */
	$object->delete();

