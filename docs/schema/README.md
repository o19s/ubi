# README

## Top-level Schemas

* [Event](./event.md "An event that occurred, typically in response to a user") – `https://o19s.github.io/ubi/schema/event.schema.json`

* [Query Request](./query.md "A query made by a user") – `https://o19s.github.io/ubi/schema/query.request.schema.json`

* [Query Response](./query-1.md "The response to a query made by a user") – `https://o19s.github.io/ubi/schema/query.response.schema.json`

## Other Schemas

### Objects

* [Untitled object in Event](./event-properties-event_attributes.md "Extensible details about a specific event") – `https://o19s.github.io/ubi/schema/event.schema.json#/properties/event_attributes`

* [Untitled object in Event](./event-properties-event_attributes-properties-object.md "Structure which contains identifying information of the object returned from the query that the user interacts with (i") – `https://o19s.github.io/ubi/schema/event.schema.json#/properties/event_attributes/properties/object`

* [Untitled object in Event](./event-properties-event_attributes-properties-position.md "Structure that contains information on the location of the event origin, such as screen x,y coordinates, or the nth object out of 10 results") – `https://o19s.github.io/ubi/schema/event.schema.json#/properties/event_attributes/properties/position`

* [Untitled object in Event](./event-properties-event_attributes-properties-position-oneof-0.md) – `https://o19s.github.io/ubi/schema/event.schema.json#/properties/event_attributes/properties/position/oneOf/0`

* [Untitled object in Event](./event-properties-event_attributes-properties-position-oneof-0-properties-ordinal.md "The nth position of the document on the search results page") – `https://o19s.github.io/ubi/schema/event.schema.json#/properties/event_attributes/properties/position/oneOf/0/properties/ordinal`

* [Untitled object in Event](./event-properties-event_attributes-properties-position-oneof-1.md) – `https://o19s.github.io/ubi/schema/event.schema.json#/properties/event_attributes/properties/position/oneOf/1`

* [Untitled object in Event](./event-properties-event_attributes-properties-position-oneof-1-properties-xy.md "The x,y coordinates on the screen for triggering an event") – `https://o19s.github.io/ubi/schema/event.schema.json#/properties/event_attributes/properties/position/oneOf/1/properties/xy`

* [Untitled object in Query Request](./query-properties-query_attributes.md "Any query modifiers like filter choices or pagination") – `https://o19s.github.io/ubi/schema/query.request.schema.json#/properties/query_attributes`

### Arrays



## Version Note

The schemas linked above follow the JSON Schema Spec version: `https://json-schema.org/draft/2020-12/schema`
