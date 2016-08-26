Cask is a high level convenience wrapper for the Alembic Python API. It blurs
the lines between Alembic “I” and “O” objects and properties, abstracting both
into a single class object. It also wraps up a number of lower-level functions
into high level convenience methods.


Basic Usage
-----------

Read an archive from disk ::

    >>> a = cask.Archive("lights.abc")

Create a new empty archive ::

    >>> b = Archive()

Deep dictionary access ::

    >>> a.top.children["root/world/lgt/gaffer/point/pointShape"]
    <Light "pointShape">
    >>> l.schema.getNumSamples()
    6


Documentation
-------------

https://alembic.github.io/cask



Installation
------------

From source ::

    $ git clone https://github.com/alembic/cask
    $ cd cask
    $ python setup.py install
