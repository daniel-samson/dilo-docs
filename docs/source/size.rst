size
====

size:value
----------

The field under validation must have a size matching the given value. For string data, value corresponds to the number of characters. For numeric data, value corresponds to a given integer value (the attribute must also have the numeric or integer rule). For an array, size corresponds to the count of the array. Let's look at some examples:

.. code-block:: javascript

    let rules = {
        // Validate that a string is exactly 12 characters long...
        'title':  'size:12',

        // Validate that a provided integer equals 10...
        'seats' :  'integer|size:10',

        // Validate that an array has exactly 5 items...
        'tags':  'array|size:5',
    }
