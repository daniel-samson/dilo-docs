Compare Rules
==============

contains:foo,bar,...
--------------------

The field under validation must be either an array that contains all of the given parameter values, or a string that contains the values given.

digits:value
------------

The integer under validation must have an exact length of value.

digits_between:min,max
----------------------

The integer validation must have a length between the given min and max.

starts_with:foo,bar,...
-----------------------

The field under validation must start with one of the given values.

doesnt_start_with:foo,bar,...
-----------------------------

The field under validation must not start with one of the given values.

ends_with:foo,bar,...
---------------------

The field under validation must end with one of the given values.

doesnt_end_with:foo,bar,...
---------------------------

The field under validation must not end with one of the given values.

email
-----

The field under validation must be formatted as an email address.

filled
------

The field under validation must not be empty when it is present.

gt:fieldOrValue
---------------

The field under validation must be greater than the given field or value. The two fields must be of the same type. Strings, numerics, arrays, and files are evaluated using the same conventions as the size rule.

gte: fieldOrValue
-----------------

The field under validation must be greater than or equal to the given field or value. The two fields must be of the same type. Strings, numerics, arrays, and files are evaluated using the same conventions as the size rule.

in:foo,bar,...
--------------

The field under validation must be included in the given list of values.

not_in:foo,bar,...
------------------

The field under validation must NOT be included in the given list of values.

lt: fieldOrValue
----------------

The field under validation must be less than the given field. The two fields must be of the same type. Strings, numerics, arrays, and files are evaluated using the same conventions as the size rule.

lte: fieldOrValue
-----------------

The field under validation must be less than or equal to the given field. The two fields must be of the same type. Strings, numerics, arrays, and files are evaluated using the same conventions as the size rule.

lowercase
---------

The field under validation must be lowercase.

uppercase
---------

The field under validation must be uppercase.

url
---

The field under validation must be a valid URL.

ulid
----

The field under validation must be a valid `Universally Unique Lexicographically Sortable Identifier <https://github.com/ulid/spec>`_ (ULID).

uuid
----

The field under validation must be a valid RFC 4122 (version 1, 3, 4, or 5) universally unique identifier (UUID).



ip
--

The field under validation must be an IP address.

ipv4
----

The field under validation must be an IPv4 address.

ipv6
----

The field under validation must be an IPv6 address.

mac_address
-----------

The field under validation must be a MAC address.
