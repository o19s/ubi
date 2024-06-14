# Untitled string in Query Tracking for UBI Schema

```txt
https://o19s.github.io/ubi/schema/1.0.0/query.request.schema.json#/properties/object_id_field
```

The name of the field that has the id of the objects that will be stored in the backend queries data store. So it you have a query for products and want to save the SKUs, then this might be `sku` and if you are querying for people, maybe this is `ssn`.  If you do not provide this value then the default primary identifier in your search index will be used.  For example `_id` on OpenSearch.

| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                      |
| :------------------ | :--------- | :------------- | :---------------------- | :---------------- | :-------------------- | :------------------ | :---------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [query.request.schema.json\*](../../out/1.0.0/query.request.schema.json "open original schema") |

## object\_id\_field Type

`string`

## object\_id\_field Constraints

**maximum length**: the maximum number of characters for this string is: `100`
