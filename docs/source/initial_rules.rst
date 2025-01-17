===============
Initial Rules
===============

When assigning the validation rules, you will likely want to start with the initial rules.

Required
--------

The field under validation must be present in the input data and not empty.

.. code-block:: javascript

    const rules = {
     foo: "required",
    };

Sometimes
---------

Run validation checks against a field only if that field is present in the data being validated.

.. code-block:: javascript

    const rules = {
     foo: "sometimes",
    };

Nullable
--------

The field under validation may be null.

.. code-block:: javascript

    const rules = {
     foo: "nullable",
    };
