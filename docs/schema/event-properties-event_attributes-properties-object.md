# Untitled object in Event tracking for UBI Schema

```txt
https://o19s.github.io/ubi/schema/X.Y.Z/event.schema.json#/properties/event_attributes/properties/object
```

Structure which contains identifying information of the object returned from the query that the user interacts with (i.e.: a book, a product, a post, etc..).

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                      |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :------------------------------------------------------------------------------ |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [event.schema.json\*](../../out/X.Y.Z/event.schema.json "open original schema") |

## object Type

`object` ([Details](event-properties-event_attributes-properties-object.md))

# object Properties

| Property                              | Type     | Required | Nullable       | Defined by                                                                                                                                                                                                                                        |
| :------------------------------------ | :------- | :------- | :------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| [object\_id](#object_id)              | Merged   | Required | cannot be null | [Event tracking for UBI](event-properties-event_attributes-properties-object-properties-object_id.md "https://o19s.github.io/ubi/schema/X.Y.Z/event.schema.json#/properties/event_attributes/properties/object/properties/object_id")             |
| [object\_id\_field](#object_id_field) | `string` | Optional | cannot be null | [Event tracking for UBI](event-properties-event_attributes-properties-object-properties-object_id_field.md "https://o19s.github.io/ubi/schema/X.Y.Z/event.schema.json#/properties/event_attributes/properties/object/properties/object_id_field") |
| [internal\_id](#internal_id)          | Merged   | Optional | cannot be null | [Event tracking for UBI](event-properties-event_attributes-properties-object-properties-internal_id.md "https://o19s.github.io/ubi/schema/X.Y.Z/event.schema.json#/properties/event_attributes/properties/object/properties/internal_id")         |
| Additional Properties                 | Any      | Optional | can be null    |                                                                                                                                                                                                                                                   |

## object\_id

The id that a user could look up and find the object instance within the *document corpus*.  Examples include: *ssn*, *isbn*, *ean*, etc. Variants need to be incorporated in the `object_id`, so for a t-shirt that is red, you would need SKU level as the `object_id`.

`object_id`

* is required

* Type: merged type ([Details](event-properties-event_attributes-properties-object-properties-object_id.md))

* cannot be null

* defined in: [Event tracking for UBI](event-properties-event_attributes-properties-object-properties-object_id.md "https://o19s.github.io/ubi/schema/X.Y.Z/event.schema.json#/properties/event_attributes/properties/object/properties/object_id")

### object\_id Type

merged type ([Details](event-properties-event_attributes-properties-object-properties-object_id.md))

any of

* [Untitled string in Event tracking for UBI](event-properties-event_attributes-properties-object-properties-object_id-anyof-0.md "check type definition")

* [Untitled integer in Event tracking for UBI](event-properties-event_attributes-properties-object-properties-object_id-anyof-1.md "check type definition")

### object\_id Examples

```json
"XYZ-12345"
```

```json
"ISBN 0-061-96436-0"
```

```json
"123"
```

## object\_id\_field

The name of the field that has the id of the objects that will be stored in the backend queries data store. So it you have a query for products and want to save the SKUs, then this might be `sku` and if you are querying for people, maybe this is `ssn`.  If you do not provide this value then the default primary identifier in your search index will be used.  For example `_id` on OpenSearch.

`object_id_field`

* is optional

* Type: `string`

* cannot be null

* defined in: [Event tracking for UBI](event-properties-event_attributes-properties-object-properties-object_id_field.md "https://o19s.github.io/ubi/schema/X.Y.Z/event.schema.json#/properties/event_attributes/properties/object/properties/object_id_field")

### object\_id\_field Type

`string`

## internal\_id

A unique id that the an individual search engine uses internally to index the object via.  For example, in OpenSearch, think the `_id` field in the indices.

`internal_id`

* is optional

* Type: merged type ([Details](event-properties-event_attributes-properties-object-properties-internal_id.md))

* cannot be null

* defined in: [Event tracking for UBI](event-properties-event_attributes-properties-object-properties-internal_id.md "https://o19s.github.io/ubi/schema/X.Y.Z/event.schema.json#/properties/event_attributes/properties/object/properties/internal_id")

### internal\_id Type

merged type ([Details](event-properties-event_attributes-properties-object-properties-internal_id.md))

any of

* [Untitled string in Event tracking for UBI](event-properties-event_attributes-properties-object-properties-internal_id-anyof-0.md "check type definition")

* [Untitled integer in Event tracking for UBI](event-properties-event_attributes-properties-object-properties-internal_id-anyof-1.md "check type definition")

### internal\_id Examples

```json
"1"
```

```json
"123456"
```

## Additional Properties

Additional properties are allowed and do not have to follow a specific schema
