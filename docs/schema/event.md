# Event tracking for UBI Schema

```txt
https://o19s.github.io/ubi/schema/X.Y.Z/event.schema.json
```

Version X.Y.Z; last updated 2024-05-23.  An event that occurred, typically in response to a user.  See [schemas.md](https://github.com/o19s/opensearch-ubi/blob/2.14.0/documentation/schemas.md) and [events-mapping.json](https://github.com/o19s/opensearch-ubi/blob/2.14.0/src/main/resources/events-mapping.json) for more info.

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                    |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :---------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [event.schema.json](../../out/X.Y.Z/event.schema.json "open original schema") |

## Event tracking for UBI Type

`object` ([Event tracking for UBI](event.md))

# Event tracking for UBI Properties

| Property                               | Type     | Required | Nullable       | Defined by                                                                                                                                              |
| :------------------------------------- | :------- | :------- | :------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------ |
| [application](#application)            | `string` | Optional | cannot be null | [Event tracking for UBI](event-properties-application.md "https://o19s.github.io/ubi/schema/X.Y.Z/event.schema.json#/properties/application")           |
| [action\_name](#action_name)           | Merged   | Required | cannot be null | [Event tracking for UBI](event-properties-action_name.md "https://o19s.github.io/ubi/schema/X.Y.Z/event.schema.json#/properties/action_name")           |
| [query\_id](#query_id)                 | Merged   | Required | cannot be null | [Event tracking for UBI](event-properties-query_id.md "https://o19s.github.io/ubi/schema/X.Y.Z/event.schema.json#/properties/query_id")                 |
| [client\_id](#client_id)               | `string` | Optional | cannot be null | [Event tracking for UBI](event-properties-client_id.md "https://o19s.github.io/ubi/schema/X.Y.Z/event.schema.json#/properties/client_id")               |
| [timestamp](#timestamp)                | `string` | Required | cannot be null | [Event tracking for UBI](event-properties-timestamp.md "https://o19s.github.io/ubi/schema/X.Y.Z/event.schema.json#/properties/timestamp")               |
| [message\_type](#message_type)         | `string` | Optional | cannot be null | [Event tracking for UBI](event-properties-message_type.md "https://o19s.github.io/ubi/schema/X.Y.Z/event.schema.json#/properties/message_type")         |
| [message](#message)                    | `string` | Optional | cannot be null | [Event tracking for UBI](event-properties-message.md "https://o19s.github.io/ubi/schema/X.Y.Z/event.schema.json#/properties/message")                   |
| [event\_attributes](#event_attributes) | `object` | Optional | cannot be null | [Event tracking for UBI](event-properties-event_attributes.md "https://o19s.github.io/ubi/schema/X.Y.Z/event.schema.json#/properties/event_attributes") |

## application

name of the application tracking UBI events.

`application`

* is optional

* Type: `string`

* cannot be null

* defined in: [Event tracking for UBI](event-properties-application.md "https://o19s.github.io/ubi/schema/X.Y.Z/event.schema.json#/properties/application")

### application Type

`string`

### application Examples

```json
"amazon-shop"
```

```json
"ABC-microservice"
```

```json
"doctor-search"
```

## action\_name

The name of the action that triggered the event.  We have a set of common defaults, however you can pass in whatever you want.

`action_name`

* is required

* Type: merged type ([Details](event-properties-action_name.md))

* cannot be null

* defined in: [Event tracking for UBI](event-properties-action_name.md "https://o19s.github.io/ubi/schema/X.Y.Z/event.schema.json#/properties/action_name")

### action\_name Type

merged type ([Details](event-properties-action_name.md))

one (and only one) of

* [Untitled string in Event tracking for UBI](event-properties-action_name-oneof-0.md "check type definition")

* [Untitled string in Event tracking for UBI](event-properties-action_name-oneof-1.md "check type definition")

## query\_id

The unique identifier of a query, typically a UUID, but can be any string.

`query_id`

* is required

* Type: merged type ([Details](event-properties-query_id.md))

* cannot be null

* defined in: [Event tracking for UBI](event-properties-query_id.md "https://o19s.github.io/ubi/schema/X.Y.Z/event.schema.json#/properties/query_id")

### query\_id Type

merged type ([Details](event-properties-query_id.md))

one (and only one) of

* [Untitled string in Event tracking for UBI](event-properties-query_id-oneof-0.md "check type definition")

* [Untitled string in Event tracking for UBI](event-properties-query_id-oneof-1.md "check type definition")

## client\_id

The client issuing the query.  This could be a unique browser, a microservice that performs searches, a crawling bot.

`client_id`

* is optional

* Type: `string`

* cannot be null

* defined in: [Event tracking for UBI](event-properties-client_id.md "https://o19s.github.io/ubi/schema/X.Y.Z/event.schema.json#/properties/client_id")

### client\_id Type

`string`

### client\_id Examples

```json
"5e3b2a1c-8b7d-4f2e-a3d4-c9b2e1f3a4b5"
```

```json
"quepid-nightly-bot"
```

```json
"BugsBunny::Firefox@0967084"
```

## timestamp

When the event took place.

`timestamp`

* is required

* Type: `string`

* cannot be null

* defined in: [Event tracking for UBI](event-properties-timestamp.md "https://o19s.github.io/ubi/schema/X.Y.Z/event.schema.json#/properties/timestamp")

### timestamp Type

`string`

### timestamp Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

### timestamp Examples

```json
"2018-11-13T20:20:39+00:00"
```

## message\_type

Group various `action_name`'s into logical bins.

> TDB: action\_type?  event\_type?  Should the front end even define this?

`message_type`

* is optional

* Type: `string`

* cannot be null

* defined in: [Event tracking for UBI](event-properties-message_type.md "https://o19s.github.io/ubi/schema/X.Y.Z/event.schema.json#/properties/message_type")

### message\_type Type

`string`

### message\_type Examples

```json
"QUERY"
```

```json
"CONVERSION"
```

## message

Optional text message for the log entry. For example, for a message\_type of QUERY, we would expect the text to be about what the user is searching on.

`message`

* is optional

* Type: `string`

* cannot be null

* defined in: [Event tracking for UBI](event-properties-message.md "https://o19s.github.io/ubi/schema/X.Y.Z/event.schema.json#/properties/message")

### message Type

`string`

### message Constraints

**maximum length**: the maximum number of characters for this string is: `1024`

## event\_attributes

Extensible details about a specific event.

`event_attributes`

* is optional

* Type: `object` ([Details](event-properties-event_attributes.md))

* cannot be null

* defined in: [Event tracking for UBI](event-properties-event_attributes.md "https://o19s.github.io/ubi/schema/X.Y.Z/event.schema.json#/properties/event_attributes")

### event\_attributes Type

`object` ([Details](event-properties-event_attributes.md))
