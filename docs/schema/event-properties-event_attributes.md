# Untitled object in Event Schema

```txt
http://github.com/o19s/ubi/schema/event.request.schema.json#/properties/event_attributes
```

Extensible details about a specific event.

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :---------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [event.request.schema.json\*](../../out/event.request.schema.json "open original schema") |

## event\_attributes Type

`object` ([Details](event-properties-event_attributes.md))

# event\_attributes Properties

| Property              | Type     | Required | Nullable       | Defined by                                                                                                                                                                       |
| :-------------------- | :------- | :------- | :------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [position](#position) | `object` | Optional | cannot be null | [Event](event-properties-event_attributes-properties-position.md "http://github.com/o19s/ubi/schema/event.request.schema.json#/properties/event_attributes/properties/position") |
| [object](#object)     | `object` | Optional | cannot be null | [Event](event-properties-event_attributes-properties-object.md "http://github.com/o19s/ubi/schema/event.request.schema.json#/properties/event_attributes/properties/object")     |

## position

structure that contains information on the location of the event origin, such as screen x,y coordinates, or the nth object out of 10 results, ....

`position`

* is optional

* Type: `object` ([Details](event-properties-event_attributes-properties-position.md))

* cannot be null

* defined in: [Event](event-properties-event_attributes-properties-position.md "http://github.com/o19s/ubi/schema/event.request.schema.json#/properties/event_attributes/properties/position")

### position Type

`object` ([Details](event-properties-event_attributes-properties-position.md))

## object

structure which contains identifying information of the object returned from the query that the user interacts with (i.e.: a book, a product, a post, etc..).

`object`

* is optional

* Type: `object` ([Details](event-properties-event_attributes-properties-object.md))

* cannot be null

* defined in: [Event](event-properties-event_attributes-properties-object.md "http://github.com/o19s/ubi/schema/event.request.schema.json#/properties/event_attributes/properties/object")

### object Type

`object` ([Details](event-properties-event_attributes-properties-object.md))
