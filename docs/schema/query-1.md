## Query Response Type

`object` ([Query Response](query-1.md))

# Query Response Properties

| Property                                                     | Type    | Required | Nullable       | Defined by                                                                                                                                                               |
| :----------------------------------------------------------- | :------ | :------- | :------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [query\_id](#query_id)                                       | Merged  | Required | cannot be null | [Query Response](query-1-properties-query_id.md "http://github.com/o19s/ubi/schema/query.response.schema.json#/properties/query_id")                                     |
| [query\_response\_objects\_ids](#query_response_objects_ids) | `array` | Optional | cannot be null | [Query Response](query-1-properties-query_response_objects_ids.md "http://github.com/o19s/ubi/schema/query.response.schema.json#/properties/query_response_objects_ids") |

## query\_id

The unique identifier of a query, typically a UUID.

`query_id`

* is required

* Type: merged type ([Details](query-1-properties-query_id.md))

* cannot be null

* defined in: [Query Response](query-1-properties-query_id.md "http://github.com/o19s/ubi/schema/query.response.schema.json#/properties/query_id")

### query\_id Type

merged type ([Details](query-1-properties-query_id.md))

one (and only one) of

* [Untitled string in Query Response](query-1-properties-query_id-oneof-0.md "check type definition")

* [Untitled string in Query Response](query-1-properties-query_id-oneof-1.md "check type definition")

## query\_response\_objects\_ids

Objects returned by the query

`query_response_objects_ids`

* is optional

* Type: an array of merged types ([Details](query-1-properties-query_response_objects_ids-items.md))

* cannot be null

* defined in: [Query Response](query-1-properties-query_response_objects_ids.md "http://github.com/o19s/ubi/schema/query.response.schema.json#/properties/query_response_objects_ids")

### query\_response\_objects\_ids Type

an array of merged types ([Details](query-1-properties-query_response_objects_ids-items.md))