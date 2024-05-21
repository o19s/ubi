# Event Schema

```txt
https://o19s.github.io/ubi/schema/event.schema.json
```

An event that occurred, typically in response to a user.  See <https://github.com/o19s/opensearch-ubi/blob/2.14.0/documentation/schemas.md> abd <https://github.com/o19s/opensearch-ubi/blob/2.14.0/src/main/resources/events-mapping.json> for more info.

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                              |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :---------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [event.schema.json](../../out/event.schema.json "open original schema") |

## Event Type

`object` ([Event](event.md))

# Event Properties

| Property                               | Type     | Required | Nullable       | Defined by                                                                                                                       |
| :------------------------------------- | :------- | :------- | :------------- | :------------------------------------------------------------------------------------------------------------------------------- |
| [application](#application)            | `string` | Optional | cannot be null | [Event](event-properties-application.md "https://o19s.github.io/ubi/schema/event.schema.json#/properties/application")           |
| [action\_name](#action_name)           | Merged   | Required | cannot be null | [Event](event-properties-action_name.md "https://o19s.github.io/ubi/schema/event.schema.json#/properties/action_name")           |
| [query\_id](#query_id)                 | Merged   | Required | cannot be null | [Event](event-properties-query_id.md "https://o19s.github.io/ubi/schema/event.schema.json#/properties/query_id")                 |
| [timestamp](#timestamp)                | `string` | Required | cannot be null | [Event](event-properties-timestamp.md "https://o19s.github.io/ubi/schema/event.schema.json#/properties/timestamp")               |
| [message\_type](#message_type)         | `string` | Optional | cannot be null | [Event](event-properties-message_type.md "https://o19s.github.io/ubi/schema/event.schema.json#/properties/message_type")         |
| [message](#message)                    | `string` | Optional | cannot be null | [Event](event-properties-message.md "https://o19s.github.io/ubi/schema/event.schema.json#/properties/message")                   |
| [event\_attributes](#event_attributes) | `object` | Optional | cannot be null | [Event](event-properties-event_attributes.md "https://o19s.github.io/ubi/schema/event.schema.json#/properties/event_attributes") |

## application

name of the application tracking UBI events (e.g. *amazon-shop*, *ABC-microservice*)

`application`

* is optional

* Type: `string`

* cannot be null

* defined in: [Event](event-properties-application.md "https://o19s.github.io/ubi/schema/event.schema.json#/properties/application")

### application Type

`string`

## action\_name

The name of the action that triggered the event.  We have a set of common defaults, however you can pass in whatever you want.

`action_name`

* is required

* Type: merged type ([Details](event-properties-action_name.md))

* cannot be null

* defined in: [Event](event-properties-action_name.md "https://o19s.github.io/ubi/schema/event.schema.json#/properties/action_name")

### action\_name Type

merged type ([Details](event-properties-action_name.md))

one (and only one) of

* [Untitled string in Event](event-properties-action_name-oneof-0.md "check type definition")

* [Untitled string in Event](event-properties-action_name-oneof-1.md "check type definition")

## query\_id

The unique identifier of a query, typically a UUID.

`query_id`

* is required

* Type: merged type ([Details](event-properties-query_id.md))

* cannot be null

* defined in: [Event](event-properties-query_id.md "https://o19s.github.io/ubi/schema/event.schema.json#/properties/query_id")

### query\_id Type

merged type ([Details](event-properties-query_id.md))

one (and only one) of

* [Untitled string in Event](event-properties-query_id-oneof-0.md "check type definition")

* [Untitled string in Event](event-properties-query_id-oneof-1.md "check type definition")

## timestamp

When the event took place.

`timestamp`

* is required

* Type: `string`

* cannot be null

* defined in: [Event](event-properties-timestamp.md "https://o19s.github.io/ubi/schema/event.schema.json#/properties/timestamp")

### timestamp Type

`string`

### timestamp Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## message\_type

ERIC: action\_type?  event\_type?  Should the front end define this?  Group various action\_name into logical bins.

`message_type`

* is optional

* Type: `string`

* cannot be null

* defined in: [Event](event-properties-message_type.md "https://o19s.github.io/ubi/schema/event.schema.json#/properties/message_type")

### message\_type Type

`string`

## message

optional text message for the log entry. For example, with a message\_type of INFO, people might expect an informational or debug type text for this field, but a message\_type of QUERY, we would expect the text to be more about what the user is searching on.

`message`

* is optional

* Type: `string`

* cannot be null

* defined in: [Event](event-properties-message.md "https://o19s.github.io/ubi/schema/event.schema.json#/properties/message")

### message Type

`string`

## event\_attributes

Extensible details about a specific event.

`event_attributes`

* is optional

* Type: `object` ([Details](event-properties-event_attributes.md))

* cannot be null

* defined in: [Event](event-properties-event_attributes.md "https://o19s.github.io/ubi/schema/event.schema.json#/properties/event_attributes")

### event\_attributes Type

`object` ([Details](event-properties-event_attributes.md))
