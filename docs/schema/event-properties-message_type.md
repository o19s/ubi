# Untitled string in Event tracking for UBI Schema

```txt
https://o19s.github.io/ubi/schema/X.Y.Z/event.schema.json#/properties/message_type
```

Group various `action_name`'s into logical bins.

> TDB: action\_type?  event\_type?  Should the front end even define this?

| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                      |
| :------------------ | :--------- | :------------- | :---------------------- | :---------------- | :-------------------- | :------------------ | :------------------------------------------------------------------------------ |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [event.schema.json\*](../../out/X.Y.Z/event.schema.json "open original schema") |

## message\_type Type

`string`

## message\_type Constraints

**maximum length**: the maximum number of characters for this string is: `100`

## message\_type Examples

```json
"QUERY"
```

```json
"CONVERSION"
```
