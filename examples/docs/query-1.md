# Query Response Schema

```txt
http://github.com/o19s/ubi/schema/query.response.schema.json
```

The response to a query made by a user.

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :---------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [query.response.schema.json](../../out/query.response.schema.json "open original schema") |

## Query Response Type

`object` ([Query Response](query-1.md))

# Query Response Properties

| Property                                                     | Type     | Required | Nullable       | Defined by                                                                                                                                                               |
| :----------------------------------------------------------- | :------- | :------- | :------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [query\_id](#query_id)                                       | `string` | Required | cannot be null | [Query Response](query-1-properties-query_id.md "http://github.com/o19s/ubi/schema/query.response.schema.json#/properties/query_id")                                     |
| [query\_response\_objects\_ids](#query_response_objects_ids) | `array`  | Optional | cannot be null | [Query Response](query-1-properties-query_response_objects_ids.md "http://github.com/o19s/ubi/schema/query.response.schema.json#/properties/query_response_objects_ids") |

## query\_id

The unique identifier of a query, typically a GUID.

`query_id`

* is required

* Type: `string`

* cannot be null

* defined in: [Query Response](query-1-properties-query_id.md "http://github.com/o19s/ubi/schema/query.response.schema.json#/properties/query_id")

### query\_id Type

`string`

## query\_response\_objects\_ids

Objects returned by the query

`query_response_objects_ids`

* is optional

* Type: an array of merged types ([Details](query-1-properties-query_response_objects_ids-items.md))

* cannot be null

* defined in: [Query Response](query-1-properties-query_response_objects_ids.md "http://github.com/o19s/ubi/schema/query.response.schema.json#/properties/query_response_objects_ids")

### query\_response\_objects\_ids Type

an array of merged types ([Details](query-1-properties-query_response_objects_ids-items.md))
