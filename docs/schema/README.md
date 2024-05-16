# README

## Top-level Schemas

* [Event](./event.md "An event that occurred, typically in response to a user") – `http://github.com/o19s/ubi/schema/event.request.schema.json`

* [Query Request](./query.md "A query made by a user") – `http://github.com/o19s/ubi/schema/query.request.schema.json`

* [Query Response](./query-1.md "The response to a query made by a user") – `http://github.com/o19s/ubi/schema/query.response.schema.json`

## Other Schemas

### Objects

* [Untitled object in Event](./event-properties-event_attributes.md "Extensible details about a specific event") – `http://github.com/o19s/ubi/schema/event.request.schema.json#/properties/event_attributes`

* [Untitled object in Event](./event-properties-event_attributes-properties-position.md "structure that contains information on the location of the event origin, such as screen x,y coordinates, or the nth object out of 10 results, ") – `http://github.com/o19s/ubi/schema/event.request.schema.json#/properties/event_attributes/properties/position`

* [Untitled object in Event](./event-properties-event_attributes-properties-object.md "structure which contains identifying information of the object returned from the query that the user interacts with (i") – `http://github.com/o19s/ubi/schema/event.request.schema.json#/properties/event_attributes/properties/object`

* [Untitled object in Query Request](./query-properties-user_query.md "ERIC: Should we require a query in user query? The query as the user entered it, plus any options they chose to change the query, like aggregation/facet choices") – `http://github.com/o19s/ubi/schema/query.request.schema.json#/properties/user_query`

### Arrays

* [Untitled array in Query Response](./query-1-properties-query_response_objects_ids.md "Objects returned by the query") – `http://github.com/o19s/ubi/schema/query.response.schema.json#/properties/query_response_objects_ids`

## Version Note

The schemas linked above follow the JSON Schema Spec version: `https://json-schema.org/draft/2020-12/schema`
