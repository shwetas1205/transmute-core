=============
Serialization
=============

transmute-core provides a framework and default implementation to
allow serializing objects to and from common data representation for
an API. This is by chaining two parts:

1. object serialization to / from basic Python data types.
2. data types serialization to / from standard data notations (e.g. json or yaml)

out of the box, object serialization is supported for:

* bool
* float
* int
* str
* decimal.Decimal
* datetime.datetime
* `schematics <http://schematics.readthedocs.org/en/latest/>`_ models.

-------------
Customization
-------------

:class:`TransmuteContext`

Both of these components are customizable, either through passing a new
TransmuteContext object, or modifying the default instance.

To learn more about customizing these serializers, please see the API reference
for TransmuteContext, ObjectSerializer, and ContentTypeSerializer.
