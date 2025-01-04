Usage
=====

.. _installation:

Installation
------------

To use Dilo, first install deno. Then you can add it to your project using deno:

.. code-block:: console

   deno add jsr:@danielsamson/dilo


Usage
----------------

.. code-block:: typescript
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



