===============
Basic Types
===============

array
-----

Validates that the field under validation is an array.

.. code-block:: javascript

    const rules = {
     foo: "array",
    };

object:list,of,keys
-------------------
The field under validation must be a typescript object. if keys specified, all of the keys must exist in the object.

.. code-block:: javascript

    const rules = {
     foo: "required|object:key1,key2", // object must be { "key1": 1, "key2": 2 }
    };

boolean
-------

The field under validation must be able to be cast as a boolean. Accepted input are true, false, 1, 0, "1", and "0"

.. code-block:: javascript

    const rules = {
     foo: "boolean",
    };

date
----

Validates that the field under validation is a date.

.. code-block:: javascript

    const rules = {
     foo: "date",
    };

decimal:min, max
----------------

The field under validation must be numeric and must contain the specified number of decimal places:

.. code-block:: javascript

    const rules = {
     foo: "required|decimal:2",
     bar: "sometimes|decimal:2,4",
    };

integer
-------

Validates that the field under validation is an integer.

.. code-block:: javascript

    const rules = {
     foo: "integer",
    };


json
----

Validates that the field under validation is a valid JSON string.

.. code-block:: javascript

    const rules = {
     foo: "json",
    };

numeric
-------

Validates that the field under validation is numeric.

.. code-block:: javascript

    const rules = {
     foo: "numeric",
    };

string
------

Validates that the field under validation is a string.

.. code-block:: javascript

    const rules = {
     foo: "string",
    };
