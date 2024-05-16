# Event

- [1. Property `Event > application`](#application)
- [2. Property `Event > action_name`](#action_name)
  - [2.1. Property `Event > action_name > oneOf > item 0`](#action_name_oneOf_i0)
  - [2.2. Property `Event > action_name > oneOf > item 1`](#action_name_oneOf_i1)
- [3. Property `Event > query_id`](#query_id)
  - [3.1. Property `Event > query_id > oneOf > item 0`](#query_id_oneOf_i0)
  - [3.2. Property `Event > query_id > oneOf > item 1`](#query_id_oneOf_i1)
- [4. Property `Event > timestamp`](#timestamp)
- [5. Property `Event > message_type`](#message_type)
- [6. Property `Event > message`](#message)
- [7. Property `Event > event_attributes`](#event_attributes)
  - [7.1. Property `Event > event_attributes > position`](#event_attributes_position)
  - [7.2. Property `Event > event_attributes > object`](#event_attributes_object)

**Title:** Event

|                           |                                                                           |
| ------------------------- | ------------------------------------------------------------------------- |
| **Type**                  | `object`                                                                  |
| **Required**              | No                                                                        |
| **Additional properties** | [[Any type: allowed]](# "Additional Properties of any type are allowed.") |

**Description:** An event that occurred, typically in response to a user.  See https://github.com/o19s/opensearch-ubi/blob/2.14.0/documentation/schemas.md abd https://github.com/o19s/opensearch-ubi/blob/2.14.0/src/main/resources/events-mapping.json for more info.

| Property                                 | Pattern | Type        | Deprecated | Definition | Title/Description                                                                                                                                                                                                                                                |
| ---------------------------------------- | ------- | ----------- | ---------- | ---------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| - [application](#application )           | No      | string      | No         | -          | name of the application tracking UBI events (e.g. _amazon-shop_, _ABC-microservice_)                                                                                                                                                                             |
| + [action_name](#action_name )           | No      | Combination | No         | -          | The name of the action that triggered the event.  We have a set of common defaults, however you can pass in whatever you want.                                                                                                                                   |
| + [query_id](#query_id )                 | No      | Combination | No         | -          | The unique identifier of a query, typically a UUID.                                                                                                                                                                                                              |
| + [timestamp](#timestamp )               | No      | string      | No         | -          | When the event took place.                                                                                                                                                                                                                                       |
| - [message_type](#message_type )         | No      | string      | No         | -          | ERIC: action_type?  event_type?  Should the front end define this?  Group various action_name into logical bins.                                                                                                                                                 |
| - [message](#message )                   | No      | string      | No         | -          | optional text message for the log entry. For example, with a message_type of INFO, people might expect an informational or debug type text for this field, but a message_type of QUERY, we would expect the text to be more about what the user is searching on. |
| - [event_attributes](#event_attributes ) | No      | object      | No         | -          | Extensible details about a specific event.                                                                                                                                                                                                                       |

## <a name="application"></a>1. Property `Event > application`

|              |          |
| ------------ | -------- |
| **Type**     | `string` |
| **Required** | No       |

**Description:** name of the application tracking UBI events (e.g. _amazon-shop_, _ABC-microservice_)

## <a name="action_name"></a>2. Property `Event > action_name`

|                           |                                                                           |
| ------------------------- | ------------------------------------------------------------------------- |
| **Type**                  | `combining`                                                               |
| **Required**              | Yes                                                                       |
| **Additional properties** | [[Any type: allowed]](# "Additional Properties of any type are allowed.") |

**Description:** The name of the action that triggered the event.  We have a set of common defaults, however you can pass in whatever you want.

| One of(Option)                  |
| ------------------------------- |
| [item 0](#action_name_oneOf_i0) |
| [item 1](#action_name_oneOf_i1) |

### <a name="action_name_oneOf_i0"></a>2.1. Property `Event > action_name > oneOf > item 0`

|              |                    |
| ------------ | ------------------ |
| **Type**     | `enum (of string)` |
| **Required** | No                 |

Must be one of:
* "click_through"
* "add_to_cart"

### <a name="action_name_oneOf_i1"></a>2.2. Property `Event > action_name > oneOf > item 1`

|              |          |
| ------------ | -------- |
| **Type**     | `string` |
| **Required** | No       |

## <a name="query_id"></a>3. Property `Event > query_id`

|                           |                                                                           |
| ------------------------- | ------------------------------------------------------------------------- |
| **Type**                  | `combining`                                                               |
| **Required**              | Yes                                                                       |
| **Additional properties** | [[Any type: allowed]](# "Additional Properties of any type are allowed.") |

**Description:** The unique identifier of a query, typically a UUID.

| One of(Option)               |
| ---------------------------- |
| [item 0](#query_id_oneOf_i0) |
| [item 1](#query_id_oneOf_i1) |

### <a name="query_id_oneOf_i0"></a>3.1. Property `Event > query_id > oneOf > item 0`

|              |          |
| ------------ | -------- |
| **Type**     | `string` |
| **Required** | No       |
| **Format**   | `uuid`   |

**Example:** 

```json
"00112233-4455-6677-8899-aabbccddeeff"
```

### <a name="query_id_oneOf_i1"></a>3.2. Property `Event > query_id > oneOf > item 1`

|              |          |
| ------------ | -------- |
| **Type**     | `string` |
| **Required** | No       |

**Example:** 

```json
"1234-user-5678"
```

## <a name="timestamp"></a>4. Property `Event > timestamp`

|              |             |
| ------------ | ----------- |
| **Type**     | `string`    |
| **Required** | Yes         |
| **Format**   | `date-time` |

**Description:** When the event took place.

## <a name="message_type"></a>5. Property `Event > message_type`

|              |          |
| ------------ | -------- |
| **Type**     | `string` |
| **Required** | No       |

**Description:** ERIC: action_type?  event_type?  Should the front end define this?  Group various action_name into logical bins.

## <a name="message"></a>6. Property `Event > message`

|              |          |
| ------------ | -------- |
| **Type**     | `string` |
| **Required** | No       |

**Description:** optional text message for the log entry. For example, with a message_type of INFO, people might expect an informational or debug type text for this field, but a message_type of QUERY, we would expect the text to be more about what the user is searching on.

## <a name="event_attributes"></a>7. Property `Event > event_attributes`

|                           |                                                                           |
| ------------------------- | ------------------------------------------------------------------------- |
| **Type**                  | `object`                                                                  |
| **Required**              | No                                                                        |
| **Additional properties** | [[Any type: allowed]](# "Additional Properties of any type are allowed.") |

**Description:** Extensible details about a specific event.

| Property                                  | Pattern | Type   | Deprecated | Definition | Title/Description                                                                                                                                             |
| ----------------------------------------- | ------- | ------ | ---------- | ---------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| - [position](#event_attributes_position ) | No      | object | No         | -          | structure that contains information on the location of the event origin, such as screen x,y coordinates, or the nth object out of 10 results, ....            |
| - [object](#event_attributes_object )     | No      | object | No         | -          | structure which contains identifying information of the object returned from the query that the user interacts with (i.e.: a book, a product, a post, etc..). |

### <a name="event_attributes_position"></a>7.1. Property `Event > event_attributes > position`

|                           |                                                                           |
| ------------------------- | ------------------------------------------------------------------------- |
| **Type**                  | `object`                                                                  |
| **Required**              | No                                                                        |
| **Additional properties** | [[Any type: allowed]](# "Additional Properties of any type are allowed.") |

**Description:** structure that contains information on the location of the event origin, such as screen x,y coordinates, or the nth object out of 10 results, ....

### <a name="event_attributes_object"></a>7.2. Property `Event > event_attributes > object`

|                           |                                                                           |
| ------------------------- | ------------------------------------------------------------------------- |
| **Type**                  | `object`                                                                  |
| **Required**              | No                                                                        |
| **Additional properties** | [[Any type: allowed]](# "Additional Properties of any type are allowed.") |

**Description:** structure which contains identifying information of the object returned from the query that the user interacts with (i.e.: a book, a product, a post, etc..).

----------------------------------------------------------------------------------------------------------------------------
Generated using [json-schema-for-humans](https://github.com/coveooss/json-schema-for-humans) on 2024-05-16 at 14:18:47 -0400
