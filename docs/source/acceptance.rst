================
Acceptance Rules
================

accepted
--------

The field under validation must be "yes", "on", 1, "1", true, or "true". This is useful for validating "Terms of Service" acceptance or similar fields.

.. code-block:: javascript

    const rules = {
     foo: "accepted",
    };

declined
--------

The field under validation must be "no", "off", 0, "0", false, or "false".

.. code-block:: javascript

    const rules = {
     foo: "declined",
    };