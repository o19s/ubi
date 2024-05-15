# Query Request

- [1. Property `Query Request > query_id`](#query_id)
  - [1.1. Property `Query Request > query_id > oneOf > item 0`](#query_id_oneOf_i0)
  - [1.2. Property `Query Request > query_id > oneOf > item 1`](#query_id_oneOf_i1)
- [2. Property `Query Request > user_query`](#user_query)

**Title:** Query Request

|                           |                                                                           |
| ------------------------- | ------------------------------------------------------------------------- |
| **Type**                  | `object`                                                                  |
| **Required**              | No                                                                        |
| **Additional properties** | [[Any type: allowed]](# "Additional Properties of any type are allowed.") |

**Description:** A query made by a user

| Property                     | Pattern | Type        | Deprecated | Definition | Title/Description                                                                                                                                                 |
| ---------------------------- | ------- | ----------- | ---------- | ---------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| - [query_id](#query_id )     | No      | Combination | No         | -          | The unique identifier of a query, typically a UUID.                                                                                                               |
| + [user_query](#user_query ) | No      | object      | No         | -          | ERIC: Should we require a query in user query? The query as the user entered it, plus any options they chose to change the query, like aggregation/facet choices. |

## <a name="query_id"></a>1. Property `Query Request > query_id`

|                           |                                                                           |
| ------------------------- | ------------------------------------------------------------------------- |
| **Type**                  | `combining`                                                               |
| **Required**              | No                                                                        |
| **Additional properties** | [[Any type: allowed]](# "Additional Properties of any type are allowed.") |

**Description:** The unique identifier of a query, typically a UUID.

| One of(Option)               |
| ---------------------------- |
| [item 0](#query_id_oneOf_i0) |
| [item 1](#query_id_oneOf_i1) |

### <a name="query_id_oneOf_i0"></a>1.1. Property `Query Request > query_id > oneOf > item 0`

|              |          |
| ------------ | -------- |
| **Type**     | `string` |
| **Required** | No       |
| **Format**   | `uuid`   |

### <a name="query_id_oneOf_i1"></a>1.2. Property `Query Request > query_id > oneOf > item 1`

|              |          |
| ------------ | -------- |
| **Type**     | `string` |
| **Required** | No       |

## <a name="user_query"></a>2. Property `Query Request > user_query`

|                           |                                                                           |
| ------------------------- | ------------------------------------------------------------------------- |
| **Type**                  | `object`                                                                  |
| **Required**              | Yes                                                                       |
| **Additional properties** | [[Any type: allowed]](# "Additional Properties of any type are allowed.") |

**Description:** ERIC: Should we require a query in user query? The query as the user entered it, plus any options they chose to change the query, like aggregation/facet choices.

| Property                                | Pattern | Type   | Deprecated | Definition | Title/Description |
| --------------------------------------- | ------- | ------ | ---------- | ---------- | ----------------- |
| - [](#user_query_additionalProperties ) | No      | object | No         | -          | -                 |

----------------------------------------------------------------------------------------------------------------------------
Generated using [json-schema-for-humans](https://github.com/coveooss/json-schema-for-humans) on 2024-05-15 at 07:57:00 -0400
