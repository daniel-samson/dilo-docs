===============
Getting Started
===============

Prerequisites
-------------

Dilo requires Deno to run. You can install Deno from https://deno.land.

Installation
------------

Then add *dilo* to your project using deno add:

.. code-block:: console

   deno add jsr:@danielsamson/dilo


Example
----------------

.. code-block:: javascript

    import { Dilo } from "@danielsamson/dilo";

    const rules = {
     foo: "required|numeric",
     bar: "sometimes|string",
     baz: "nullable|boolean",
    };

    const request = Dilo.make(rules);
    const errors = request.validate({ foo: "1", bar: "bar", baz: true });

    if (errors) {
     for (const field of Object.keys(errors)) {
      console.log(field, errors[field]);
     }
    }



