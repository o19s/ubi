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

| Property                   | Type     | Required | Nullable       | Defined by                                                                                                                           |
| :------------------------- | :------- | :------- | :------------- | :----------------------------------------------------------------------------------------------------------------------------------- |
| [query\_id](#query_id)     | Merged   | Optional | cannot be null | [Query Request](query-properties-query_id.md "http://github.com/o19s/ubi/schema/query.request.schema.json#/properties/query_id")     |
| [user\_query](#user_query) | `object` | Required | cannot be null | [Query Request](query-properties-user_query.md "http://github.com/o19s/ubi/schema/query.request.schema.json#/properties/user_query") |

## query\_id

The unique identifier of a query, typically a UUID.

`query_id`

* is optional

* Type: merged type ([Details](query-properties-query_id.md))

* cannot be null

* defined in: [Query Request](query-properties-query_id.md "http://github.com/o19s/ubi/schema/query.request.schema.json#/properties/query_id")

### query\_id Type

merged type ([Details](query-properties-query_id.md))

one (and only one) of

* [Untitled string in Query Request](query-properties-query_id-oneof-0.md "check type definition")

* [Untitled string in Query Request](query-properties-query_id-oneof-1.md "check type definition")

## user\_query

ERIC: Should we require a query in user query? The query as the user entered it, plus any options they chose to change the query, like aggregation/facet choices.

`user_query`

* is required

* Type: `object` ([Details](query-properties-user_query.md))

* cannot be null

* defined in: [Query Request](query-properties-user_query.md "http://github.com/o19s/ubi/schema/query.request.schema.json#/properties/user_query")

### user\_query Type

`object` ([Details](query-properties-user_query.md))
