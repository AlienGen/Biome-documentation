.. biome:

Biome
*****

Biome
=====

Workflow
--------

.. graphviz::

	digraph {
		"Autoload" -> "Initialize services";
		"Initialize services" -> "Routing";
		"Routing" -> "Controller";
		"Controller" -> "Load view";
		"Load view" -> "Rendering";
		"Rendering" -> "Output";
	}

Services
--------

Router
======

Controller
==========

Method
------

Action
------

Parameters injection

Collection
==========

RequestCollection
-----------------

SessionCollection
-----------------

Logging
=======

Caching
=======

Command
=======

Translation
===========

Validation
==========

