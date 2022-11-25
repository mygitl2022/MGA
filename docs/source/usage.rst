MEGA Usage
=====

.. _installation:

Installation
------------

To use MEGA, first install it using pip:

.. code-block:: console

   (.venv) $ pip install mega

Creating recipes
----------------

To retrieve a list of random ingredients,
you can use the ``mega.get_random_ingredients()`` function:

.. autofunction:: mega.get_random_ingredients

The ``kind`` parameter should be either ``"meat"``, ``"fish"``,
or ``"veggies"``. Otherwise, :py:func:`mega.get_random_ingredients`
will raise an exception.

.. autoexception:: mega.InvalidKindError

For example:

>>> import mega
>>> mega.get_random_ingredients()
['shells', 'gorgonzola', 'parsley']

