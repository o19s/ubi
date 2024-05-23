# Untitled undefined type in Event tracking for UBI Schema

```txt
https://o19s.github.io/ubi/schema/X.Y.Z/event.schema.json#/properties/event_attributes/properties/object/properties/object_id
```

The id that a user could look up and find the object instance within the *document corpus*.  Examples include: *ssn*, *isbn*, *ean*, etc. Variants need to be incorporated in the `object_id`, so for a t-shirt that is red, you would need SKU level as the `object_id`.

| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                      |
| :------------------ | :--------- | :------------- | :---------------------- | :---------------- | :-------------------- | :------------------ | :------------------------------------------------------------------------------ |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [event.schema.json\*](../../out/X.Y.Z/event.schema.json "open original schema") |

## object\_id Type

merged type ([Details](event-properties-event_attributes-properties-object-properties-object_id.md))

any of

* [Untitled string in Event tracking for UBI](event-properties-event_attributes-properties-object-properties-object_id-anyof-0.md "check type definition")

* [Untitled integer in Event tracking for UBI](event-properties-event_attributes-properties-object-properties-object_id-anyof-1.md "check type definition")

## object\_id Examples

```json
"XYZ-12345"
```

```json
"ISBN 0-061-96436-0"
```

```json
"123"
```
