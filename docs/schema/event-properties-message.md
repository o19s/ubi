# Untitled string in Event Schema

```txt
http://github.com/o19s/ubi/schema/event.request.schema.json#/properties/message
```

optional text message for the log entry. For example, with a message\_type of INFO, people might expect an informational or debug type text for this field, but a message\_type of QUERY, we would expect the text to be more about what the user is searching on.

| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                |
| :------------------ | :--------- | :------------- | :---------------------- | :---------------- | :-------------------- | :------------------ | :---------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [event.request.schema.json\*](../../out/event.request.schema.json "open original schema") |

## message Type

`string`
