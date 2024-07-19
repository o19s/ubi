# Untitled object in Event tracking for UBI Schema

```txt
https://o19s.github.io/ubi/schema/1.0.0/event.schema.json#/properties/event_attributes
```

Extensible details about a specific event. A common example of an  *Additional Properties* is the specific identifier of the user (`user_id`).  Note: a user identifier is different then the required `client_id` attribute.

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                      |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :------------------------------------------------------------------------------ |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [event.schema.json\*](../../out/1.0.0/event.schema.json "open original schema") |

## event\_attributes Type

`object` ([Details](event-properties-event_attributes.md))

# event\_attributes Properties

| Property              | Type     | Required | Nullable       | Defined by                                                                                                                                                                                      |
| :-------------------- | :------- | :------- | :------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [object](#object)     | `object` | Optional | cannot be null | [Event tracking for UBI](event-properties-event_attributes-properties-object.md "https://o19s.github.io/ubi/schema/1.0.0/event.schema.json#/properties/event_attributes/properties/object")     |
| [position](#position) | Merged   | Required | cannot be null | [Event tracking for UBI](event-properties-event_attributes-properties-position.md "https://o19s.github.io/ubi/schema/1.0.0/event.schema.json#/properties/event_attributes/properties/position") |
| Additional Properties | Any      | Optional | can be null    |                                                                                                                                                                                                 |

## object

Structure which contains identifying information of the object returned from the query that the user interacts with (i.e.: a book, a product, a post, etc..).

`object`

* is optional

* Type: `object` ([Details](event-properties-event_attributes-properties-object.md))

* cannot be null

* defined in: [Event tracking for UBI](event-properties-event_attributes-properties-object.md "https://o19s.github.io/ubi/schema/1.0.0/event.schema.json#/properties/event_attributes/properties/object")

### object Type

`object` ([Details](event-properties-event_attributes-properties-object.md))

## position

Structure that contains information on the location of the event origin, such as screen x,y coordinates, or the nth object out of 10 results.

`position`

* is required

* Type: `object` ([Details](event-properties-event_attributes-properties-position.md))

* cannot be null

* defined in: [Event tracking for UBI](event-properties-event_attributes-properties-position.md "https://o19s.github.io/ubi/schema/1.0.0/event.schema.json#/properties/event_attributes/properties/position")

### position Type

`object` ([Details](event-properties-event_attributes-properties-position.md))

one (and only one) of

* [Untitled object in Event tracking for UBI](event-properties-event_attributes-properties-position-oneof-0.md "check type definition")

* [Untitled object in Event tracking for UBI](event-properties-event_attributes-properties-position-oneof-1.md "check type definition")

## Additional Properties

Additional properties are allowed and do not have to follow a specific schema
