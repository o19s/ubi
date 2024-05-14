# Event Schema

```txt
http://github.com/o19s/ubi/schema/event.request.schema.json
```

An event that occurred, typically in response to a user.  See <https://github.com/o19s/opensearch-ubi/blob/2.14.0/src/main/resources/events-mapping.json> for more info.

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                              |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :-------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [event.request.schema.json](../../out/event.request.schema.json "open original schema") |

## Event Type

`object` ([Event](event.md))

# Event Properties

| Property                     | Type     | Required | Nullable       | Defined by                                                                                                                     |
| :--------------------------- | :------- | :------- | :------------- | :----------------------------------------------------------------------------------------------------------------------------- |
| [application](#application)  | `string` | Optional | cannot be null | [Event](event-properties-application.md "http://github.com/o19s/ubi/schema/event.request.schema.json#/properties/application") |
| [action\_name](#action_name) | Merged   | Optional | cannot be null | [Event](event-properties-action_name.md "http://github.com/o19s/ubi/schema/event.request.schema.json#/properties/action_name") |
| [query\_id](#query_id)       | Merged   | Optional | cannot be null | [Event](event-properties-query_id.md "http://github.com/o19s/ubi/schema/event.request.schema.json#/properties/query_id")       |
| [timestamp](#timestamp)      | `string` | Optional | cannot be null | [Event](event-properties-timestamp.md "http://github.com/o19s/ubi/schema/event.request.schema.json#/properties/timestamp")     |

## application

name of the application tracking UBI events (e.g. *amazon-shop*, *ABC-microservice*)

`application`

* is optional

* Type: `string`

* cannot be null

* defined in: [Event](event-properties-application.md "http://github.com/o19s/ubi/schema/event.request.schema.json#/properties/application")

### application Type

`string`

## action\_name

The name of the action that triggered the event.  We have a set of common defaults, however you can pass in whatever you want.

`action_name`

* is optional

* Type: merged type ([Details](event-properties-action_name.md))

* cannot be null

* defined in: [Event](event-properties-action_name.md "http://github.com/o19s/ubi/schema/event.request.schema.json#/properties/action_name")

### action\_name Type

merged type ([Details](event-properties-action_name.md))

one (and only one) of

* [Untitled string in Event](event-properties-action_name-oneof-0.md "check type definition")

* [Untitled string in Event](event-properties-action_name-oneof-1.md "check type definition")

## query\_id

The unique identifier of a query, typically a UUID.

`query_id`

* is optional

* Type: merged type ([Details](event-properties-query_id.md))

* cannot be null

* defined in: [Event](event-properties-query_id.md "http://github.com/o19s/ubi/schema/event.request.schema.json#/properties/query_id")

### query\_id Type

merged type ([Details](event-properties-query_id.md))

one (and only one) of

* [Untitled string in Event](event-properties-query_id-oneof-0.md "check type definition")

* [Untitled string in Event](event-properties-query_id-oneof-1.md "check type definition")

## timestamp

When the event took place.

`timestamp`

* is optional

* Type: `string`

* cannot be null

* defined in: [Event](event-properties-timestamp.md "http://github.com/o19s/ubi/schema/event.request.schema.json#/properties/timestamp")

### timestamp Type

`string`

### timestamp Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")
