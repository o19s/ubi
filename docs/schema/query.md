# Query Request Schema

```txt
http://github.com/o19s/ubi/schema/query.request.schema.json
```

A query made by a user

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                              |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :-------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [query.request.schema.json](../../out/query.request.schema.json "open original schema") |

## Query Request Type

`object` ([Query Request](query.md))

# Query Request Properties

| Property               | Type     | Required | Nullable       | Defined by                                                                                                                       |
| :--------------------- | :------- | :------- | :------------- | :------------------------------------------------------------------------------------------------------------------------------- |
| [query\_id](#query_id) | `string` | Optional | cannot be null | [Query Request](query-properties-query_id.md "http://github.com/o19s/ubi/schema/query.request.schema.json#/properties/query_id") |

## query\_id

The unique identifier of a query, typically a GUID.

`query_id`

* is optional

* Type: `string`

* cannot be null

* defined in: [Query Request](query-properties-query_id.md "http://github.com/o19s/ubi/schema/query.request.schema.json#/properties/query_id")

### query\_id Type

`string`
