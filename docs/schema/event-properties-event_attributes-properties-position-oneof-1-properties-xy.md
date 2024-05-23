# Untitled object in Event tracking for UBI Schema

```txt
https://o19s.github.io/ubi/schema/X.Y.Z/event.schema.json#/properties/event_attributes/properties/position/oneOf/1/properties/xy
```

The x,y coordinates on the screen for triggering an event.

> What about bounding boxes?

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                      |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :------------------------------------------------------------------------------ |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [event.schema.json\*](../../out/X.Y.Z/event.schema.json "open original schema") |

## xy Type

`object` ([Details](event-properties-event_attributes-properties-position-oneof-1-properties-xy.md))

# xy Properties

| Property | Type     | Required | Nullable       | Defined by                                                                                                                                                                                                                                                            |
| :------- | :------- | :------- | :------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [x](#x)  | `number` | Required | cannot be null | [Event tracking for UBI](event-properties-event_attributes-properties-position-oneof-1-properties-xy-properties-x.md "https://o19s.github.io/ubi/schema/X.Y.Z/event.schema.json#/properties/event_attributes/properties/position/oneOf/1/properties/xy/properties/x") |
| [y](#y)  | `number` | Required | cannot be null | [Event tracking for UBI](event-properties-event_attributes-properties-position-oneof-1-properties-xy-properties-y.md "https://o19s.github.io/ubi/schema/X.Y.Z/event.schema.json#/properties/event_attributes/properties/position/oneOf/1/properties/xy/properties/y") |

## x

The horizontal location on the page or screen of the event.

`x`

* is required

* Type: `number`

* cannot be null

* defined in: [Event tracking for UBI](event-properties-event_attributes-properties-position-oneof-1-properties-xy-properties-x.md "https://o19s.github.io/ubi/schema/X.Y.Z/event.schema.json#/properties/event_attributes/properties/position/oneOf/1/properties/xy/properties/x")

### x Type

`number`

## y

The vertical location on the page or screen of the event.

`y`

* is required

* Type: `number`

* cannot be null

* defined in: [Event tracking for UBI](event-properties-event_attributes-properties-position-oneof-1-properties-xy-properties-y.md "https://o19s.github.io/ubi/schema/X.Y.Z/event.schema.json#/properties/event_attributes/properties/position/oneOf/1/properties/xy/properties/y")

### y Type

`number`
