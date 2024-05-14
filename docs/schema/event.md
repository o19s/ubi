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
| [action\_name](#action_name) | `string` | Optional | cannot be null | [Event](event-properties-action_name.md "http://github.com/o19s/ubi/schema/event.request.schema.json#/properties/action_name") |
| [query\_id](#query_id)       | `string` | Optional | cannot be null | [Event](event-properties-query_id.md "http://github.com/o19s/ubi/schema/event.request.schema.json#/properties/query_id")       |
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

Eric: should have an anyOf with an enum.  .any name you want to call your event. For example, with javascript events, you could include on\_click, logon, add\_to\_cart, page\_scroll

`action_name`

* is optional

* Type: `string`

* cannot be null

* defined in: [Event](event-properties-action_name.md "http://github.com/o19s/ubi/schema/event.request.schema.json#/properties/action_name")

### action\_name Type

`string`

## query\_id

The unique identifier of a query, typically a GUID.

`query_id`

* is optional

* Type: `string`

* cannot be null

* defined in: [Event](event-properties-query_id.md "http://github.com/o19s/ubi/schema/event.request.schema.json#/properties/query_id")

### query\_id Type

`string`

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
