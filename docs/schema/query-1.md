# Query Response Schema

```txt
https://o19s.github.io/ubi/schema/query.response.schema.json
```

The response to a query made by a user.

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :---------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [query.response.schema.json](../../out/query.response.schema.json "open original schema") |

## Query Response Type

`object` ([Query Response](query-1.md))

# Query Response Properties

| Property               | Type   | Required | Nullable       | Defined by                                                                                                                           |
| :--------------------- | :----- | :------- | :------------- | :----------------------------------------------------------------------------------------------------------------------------------- |
| [query\_id](#query_id) | Merged | Required | cannot be null | [Query Response](query-1-properties-query_id.md "https://o19s.github.io/ubi/schema/query.response.schema.json#/properties/query_id") |

## query\_id

The unique identifier of a query, typically a UUID, but can be any string.

`query_id`

* is required

* Type: merged type ([Details](query-1-properties-query_id.md))

* cannot be null

* defined in: [Query Response](query-1-properties-query_id.md "https://o19s.github.io/ubi/schema/query.response.schema.json#/properties/query_id")

### query\_id Type

merged type ([Details](query-1-properties-query_id.md))

one (and only one) of

* [Untitled string in Query Response](query-1-properties-query_id-oneof-0.md "check type definition")

* [Untitled string in Query Response](query-1-properties-query_id-oneof-1.md "check type definition")
