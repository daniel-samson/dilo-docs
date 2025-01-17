Field Rules
===========


missing
-------
The field under validation must not be present in the input data.

missing_if:anotherfield,value,...
---------------------------------

The field under validation must not be present if the anotherfield field is equal to any value.

missing_unless:anotherfield,value
---------------------------------

The field under validation must not be present unless the anotherfield field is equal to any value.

missing_with:foo,bar,...
------------------------

The field under validation must not be present only if any of the other specified fields are present.

missing_with_all:foo,bar,...
----------------------------

The field under validation must not be present only if all of the other specified fields are present.

same:field
----------
The given field must match the field under validation.