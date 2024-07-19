# Untitled string in Event tracking for UBI Schema

```txt
https://o19s.github.io/ubi/schema/1.0.0/event.schema.json#/properties/client_id
```

The client issuing the query.  This could be a unique browser, a microservice that performs searches, a crawling bot. If only authenticated users are tracked, then you could use a specific user id here, otherwise you should use something permanent and track user id as an *Additional Property*.

| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                      |
| :------------------ | :--------- | :------------- | :---------------------- | :---------------- | :-------------------- | :------------------ | :------------------------------------------------------------------------------ |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [event.schema.json\*](../../out/1.0.0/event.schema.json "open original schema") |

## client\_id Type

`string`

## client\_id Constraints

**maximum length**: the maximum number of characters for this string is: `100`

## client\_id Examples

```json
"5e3b2a1c-8b7d-4f2e-a3d4-c9b2e1f3a4b5"
```

```json
"quepid-nightly-bot"
```

```json
"BugsBunny::Firefox@0967084"
```
