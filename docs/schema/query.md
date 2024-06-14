# Query Response When Using UBI Schema

```txt
https://o19s.github.io/ubi/schema/1.0.0/query.response.schema.json
```

Version 1.0.0; last updated 2024-06-14.  The response to a query made by a user should support this schema.

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                      |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :---------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [query.response.schema.json](../../out/1.0.0/query.response.schema.json "open original schema") |

## Query Response When Using UBI Type

`object` ([Query Response When Using UBI](query.md))

# Query Response When Using UBI Properties

| Property               | Type   | Required | Nullable       | Defined by                                                                                                                                              |
| :--------------------- | :----- | :------- | :------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------ |
| [query\_id](#query_id) | Merged | Required | cannot be null | [Query Response When Using UBI](query-properties-query_id.md "https://o19s.github.io/ubi/schema/1.0.0/query.response.schema.json#/properties/query_id") |

## query\_id

The unique identifier of a query, typically a UUID, but can be any string.

`query_id`

* is required

* Type: merged type ([Details](query-properties-query_id.md))

* cannot be null

* defined in: [Query Response When Using UBI](query-properties-query_id.md "https://o19s.github.io/ubi/schema/1.0.0/query.response.schema.json#/properties/query_id")

### query\_id Type

merged type ([Details](query-properties-query_id.md))

one (and only one) of

* [Untitled string in Query Response When Using UBI](query-properties-query_id-oneof-0.md "check type definition")

* [Untitled string in Query Response When Using UBI](query-properties-query_id-oneof-1.md "check type definition")
