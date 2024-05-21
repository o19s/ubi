# Query Request Schema

```txt
https://o19s.github.io/ubi/schema/query.request.schema.json
```

A query made by a user

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                              |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :-------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [query.request.schema.json](../../out/query.request.schema.json "open original schema") |

## Query Request Type

`object` ([Query Request](query.md))

# Query Request Properties

| Property                               | Type     | Required | Nullable       | Defined by                                                                                                                                       |
| :------------------------------------- | :------- | :------- | :------------- | :----------------------------------------------------------------------------------------------------------------------------------------------- |
| [query\_id](#query_id)                 | Merged   | Optional | cannot be null | [Query Request](query-properties-query_id.md "https://o19s.github.io/ubi/schema/query.request.schema.json#/properties/query_id")                 |
| [user\_query](#user_query)             | `string` | Required | cannot be null | [Query Request](query-properties-user_query.md "https://o19s.github.io/ubi/schema/query.request.schema.json#/properties/user_query")             |
| [query\_attributes](#query_attributes) | `object` | Optional | cannot be null | [Query Request](query-properties-query_attributes.md "https://o19s.github.io/ubi/schema/query.request.schema.json#/properties/query_attributes") |

## query\_id

The unique identifier of a query, typically a UUID, but can be any string.

`query_id`

* is optional

* Type: merged type ([Details](query-properties-query_id.md))

* cannot be null

* defined in: [Query Request](query-properties-query_id.md "https://o19s.github.io/ubi/schema/query.request.schema.json#/properties/query_id")

### query\_id Type

merged type ([Details](query-properties-query_id.md))

one (and only one) of

* [Untitled string in Query Request](query-properties-query_id-oneof-0.md "check type definition")

* [Untitled string in Query Request](query-properties-query_id-oneof-1.md "check type definition")

## user\_query

The query as the user entered it.

> Currently not required to support recommendation systems etc that might not have a user generated query.

`user_query`

* is required

* Type: `string`

* cannot be null

* defined in: [Query Request](query-properties-user_query.md "https://o19s.github.io/ubi/schema/query.request.schema.json#/properties/user_query")

### user\_query Type

`string`

## query\_attributes

Any query modifiers like filter choices or pagination. Other attributes such as experiment identifiers that need to be tracked with the query.

`query_attributes`

* is optional

* Type: `object` ([Details](query-properties-query_attributes.md))

* cannot be null

* defined in: [Query Request](query-properties-query_attributes.md "https://o19s.github.io/ubi/schema/query.request.schema.json#/properties/query_attributes")

### query\_attributes Type

`object` ([Details](query-properties-query_attributes.md))
