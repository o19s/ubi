# Query Tracking for UBI Schema

```txt
https://o19s.github.io/ubi/schema/X.Y.Z/query.request.schema.json
```

Version X.Y.Z; last updated 2024-05-23.  A query made by a user should include these attributes for UBI tracking.

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                    |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :-------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [query.request.schema.json](../../out/X.Y.Z/query.request.schema.json "open original schema") |

## Query Tracking for UBI Type

`object` ([Query Tracking for UBI](query-1.md))

# Query Tracking for UBI Properties

| Property                               | Type     | Required | Nullable       | Defined by                                                                                                                                                        |
| :------------------------------------- | :------- | :------- | :------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [query\_id](#query_id)                 | Merged   | Optional | cannot be null | [Query Tracking for UBI](query-1-properties-query_id.md "https://o19s.github.io/ubi/schema/X.Y.Z/query.request.schema.json#/properties/query_id")                 |
| [client\_id](#client_id)               | `string` | Optional | cannot be null | [Query Tracking for UBI](query-1-properties-client_id.md "https://o19s.github.io/ubi/schema/X.Y.Z/query.request.schema.json#/properties/client_id")               |
| [user\_query](#user_query)             | `string` | Required | cannot be null | [Query Tracking for UBI](query-1-properties-user_query.md "https://o19s.github.io/ubi/schema/X.Y.Z/query.request.schema.json#/properties/user_query")             |
| [query\_attributes](#query_attributes) | `object` | Optional | cannot be null | [Query Tracking for UBI](query-1-properties-query_attributes.md "https://o19s.github.io/ubi/schema/X.Y.Z/query.request.schema.json#/properties/query_attributes") |
| [object\_id\_field](#object_id_field)  | `string` | Optional | cannot be null | [Query Tracking for UBI](query-1-properties-object_id_field.md "https://o19s.github.io/ubi/schema/X.Y.Z/query.request.schema.json#/properties/object_id_field")   |

## query\_id

The unique identifier of a query, typically a UUID, but can be any string.

`query_id`

* is optional

* Type: merged type ([Details](query-1-properties-query_id.md))

* cannot be null

* defined in: [Query Tracking for UBI](query-1-properties-query_id.md "https://o19s.github.io/ubi/schema/X.Y.Z/query.request.schema.json#/properties/query_id")

### query\_id Type

merged type ([Details](query-1-properties-query_id.md))

one (and only one) of

* [Untitled string in Query Tracking for UBI](query-1-properties-query_id-oneof-0.md "check type definition")

* [Untitled string in Query Tracking for UBI](query-1-properties-query_id-oneof-1.md "check type definition")

## client\_id

The client issuing the query.  This could be a unique browser, a microservice that performs searches, a crawling bot.

`client_id`

* is optional

* Type: `string`

* cannot be null

* defined in: [Query Tracking for UBI](query-1-properties-client_id.md "https://o19s.github.io/ubi/schema/X.Y.Z/query.request.schema.json#/properties/client_id")

### client\_id Type

`string`

### client\_id Examples

```json
"5e3b2a1c-8b7d-4f2e-a3d4-c9b2e1f3a4b5"
```

```json
"quepid-nightly-bot"
```

```json
"BugsBunny::Firefox@0967084"
```

## user\_query

The query as the user entered it.

> Currently not required to support recommendation systems etc that might not have a user generated query.

`user_query`

* is required

* Type: `string`

* cannot be null

* defined in: [Query Tracking for UBI](query-1-properties-user_query.md "https://o19s.github.io/ubi/schema/X.Y.Z/query.request.schema.json#/properties/user_query")

### user\_query Type

`string`

## query\_attributes

Any query modifiers like filter choices or pagination. Other attributes such as experiment identifiers that need to be tracked with the query.

`query_attributes`

* is optional

* Type: `object` ([Details](query-1-properties-query_attributes.md))

* cannot be null

* defined in: [Query Tracking for UBI](query-1-properties-query_attributes.md "https://o19s.github.io/ubi/schema/X.Y.Z/query.request.schema.json#/properties/query_attributes")

### query\_attributes Type

`object` ([Details](query-1-properties-query_attributes.md))

## object\_id\_field

The name of the field that has the id of the objects that will be stored in the backend queries data store. So it you have a query for products and want to save the SKUs, then this might be `sku` and if you are querying for people, maybe this is `ssn`.  If you do not provide this value then the default primary identifier in your search index will be used.  For example `_id` on OpenSearch.

`object_id_field`

* is optional

* Type: `string`

* cannot be null

* defined in: [Query Tracking for UBI](query-1-properties-object_id_field.md "https://o19s.github.io/ubi/schema/X.Y.Z/query.request.schema.json#/properties/object_id_field")

### object\_id\_field Type

`string`
