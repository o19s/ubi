<a name="#resource-app"></a>
## App

Stability: `prototype`

FIXME


### Attributes

<details>
  <summary>Details</summary>


| Name | Type | Description | Example |
| ------- | ------- | ------- | ------- |
| **created_at** | *date-time* | when app was created | `"2015-01-01T12:00:00Z"` |
| **id** | *uuid* | unique identifier of app | `"01234567-89ab-cdef-0123-456789abcdef"` |
| **name** | *string* | unique name of app | `"example"` |
| **updated_at** | *date-time* | when app was updated | `"2015-01-01T12:00:00Z"` |

</details>

<a name="link-POST-app-/apps"></a>
### App Create

<details>
  <summary>Details</summary>

Create a new app.

```
POST /apps
```


#### Curl Example

```bash
$ curl -n -X POST https://api.hello.com/apps \
  -d '{
}' \
  -H "Content-Type: application/json"
```


#### Response Example

```
HTTP/1.1 201 Created
```

```json
{
  "created_at": "2015-01-01T12:00:00Z",
  "id": "01234567-89ab-cdef-0123-456789abcdef",
  "name": "example",
  "updated_at": "2015-01-01T12:00:00Z"
}
```

</details>

<a name="link-DELETE-app-/apps/{(%23%2Fdefinitions%2Fapp%2Fdefinitions%2Fidentity)}"></a>
### App Delete

<details>
  <summary>Details</summary>

Delete an existing app.

```
DELETE /apps/{app_id_or_name}
```


#### Curl Example

```bash
$ curl -n -X DELETE https://api.hello.com/apps/$APP_ID_OR_NAME \
  -H "Content-Type: application/json"
```


#### Response Example

```
HTTP/1.1 200 OK
```

```json
{
  "created_at": "2015-01-01T12:00:00Z",
  "id": "01234567-89ab-cdef-0123-456789abcdef",
  "name": "example",
  "updated_at": "2015-01-01T12:00:00Z"
}
```

</details>

<a name="link-GET-app-/apps/{(%23%2Fdefinitions%2Fapp%2Fdefinitions%2Fidentity)}"></a>
### App Info

<details>
  <summary>Details</summary>

Info for existing app.

```
GET /apps/{app_id_or_name}
```


#### Curl Example

```bash
$ curl -n https://api.hello.com/apps/$APP_ID_OR_NAME
```


#### Response Example

```
HTTP/1.1 200 OK
```

```json
{
  "created_at": "2015-01-01T12:00:00Z",
  "id": "01234567-89ab-cdef-0123-456789abcdef",
  "name": "example",
  "updated_at": "2015-01-01T12:00:00Z"
}
```

</details>

<a name="link-GET-app-/apps"></a>
### App List

<details>
  <summary>Details</summary>

List existing apps.

```
GET /apps
```


#### Curl Example

```bash
$ curl -n https://api.hello.com/apps
```


#### Response Example

```
HTTP/1.1 200 OK
```

```json
[
  {
    "created_at": "2015-01-01T12:00:00Z",
    "id": "01234567-89ab-cdef-0123-456789abcdef",
    "name": "example",
    "updated_at": "2015-01-01T12:00:00Z"
  }
]
```

</details>

<a name="link-PATCH-app-/apps/{(%23%2Fdefinitions%2Fapp%2Fdefinitions%2Fidentity)}"></a>
### App Update

<details>
  <summary>Details</summary>

Update an existing app.

```
PATCH /apps/{app_id_or_name}
```


#### Curl Example

```bash
$ curl -n -X PATCH https://api.hello.com/apps/$APP_ID_OR_NAME \
  -d '{
}' \
  -H "Content-Type: application/json"
```


#### Response Example

```
HTTP/1.1 200 OK
```

```json
{
  "created_at": "2015-01-01T12:00:00Z",
  "id": "01234567-89ab-cdef-0123-456789abcdef",
  "name": "example",
  "updated_at": "2015-01-01T12:00:00Z"
}
```

</details>


<a name="#resource-user"></a>
## User

Stability: `prototype`

FIXME


### Attributes

<details>
  <summary>Details</summary>


| Name | Type | Description | Example |
| ------- | ------- | ------- | ------- |
| **created_at** | *date-time* | when user was created | `"2015-01-01T12:00:00Z"` |
| **id** | *uuid* | unique identifier of user | `"01234567-89ab-cdef-0123-456789abcdef"` |
| **name** | *string* | unique name of user | `"example"` |
| **updated_at** | *date-time* | when user was updated | `"2015-01-01T12:00:00Z"` |

</details>

<a name="link-POST-user-/users"></a>
### User Create

<details>
  <summary>Details</summary>

Create a new user.

```
POST /users
```


#### Curl Example

```bash
$ curl -n -X POST https://api.hello.com/users \
  -d '{
}' \
  -H "Content-Type: application/json"
```


#### Response Example

```
HTTP/1.1 201 Created
```

```json
{
  "created_at": "2015-01-01T12:00:00Z",
  "id": "01234567-89ab-cdef-0123-456789abcdef",
  "name": "example",
  "updated_at": "2015-01-01T12:00:00Z"
}
```

</details>

<a name="link-DELETE-user-/users/{(%23%2Fdefinitions%2Fuser%2Fdefinitions%2Fidentity)}"></a>
### User Delete

<details>
  <summary>Details</summary>

Delete an existing user.

```
DELETE /users/{user_id_or_name}
```


#### Curl Example

```bash
$ curl -n -X DELETE https://api.hello.com/users/$USER_ID_OR_NAME \
  -H "Content-Type: application/json"
```


#### Response Example

```
HTTP/1.1 200 OK
```

```json
{
  "created_at": "2015-01-01T12:00:00Z",
  "id": "01234567-89ab-cdef-0123-456789abcdef",
  "name": "example",
  "updated_at": "2015-01-01T12:00:00Z"
}
```

</details>

<a name="link-GET-user-/users/{(%23%2Fdefinitions%2Fuser%2Fdefinitions%2Fidentity)}"></a>
### User Info

<details>
  <summary>Details</summary>

Info for existing user.

```
GET /users/{user_id_or_name}
```


#### Curl Example

```bash
$ curl -n https://api.hello.com/users/$USER_ID_OR_NAME
```


#### Response Example

```
HTTP/1.1 200 OK
```

```json
{
  "created_at": "2015-01-01T12:00:00Z",
  "id": "01234567-89ab-cdef-0123-456789abcdef",
  "name": "example",
  "updated_at": "2015-01-01T12:00:00Z"
}
```

</details>

<a name="link-GET-user-/users"></a>
### User List

<details>
  <summary>Details</summary>

List existing users.

```
GET /users
```


#### Curl Example

```bash
$ curl -n https://api.hello.com/users
```


#### Response Example

```
HTTP/1.1 200 OK
```

```json
[
  {
    "created_at": "2015-01-01T12:00:00Z",
    "id": "01234567-89ab-cdef-0123-456789abcdef",
    "name": "example",
    "updated_at": "2015-01-01T12:00:00Z"
  }
]
```

</details>

<a name="link-PATCH-user-/users/{(%23%2Fdefinitions%2Fuser%2Fdefinitions%2Fidentity)}"></a>
### User Update

<details>
  <summary>Details</summary>

Update an existing user.

```
PATCH /users/{user_id_or_name}
```


#### Curl Example

```bash
$ curl -n -X PATCH https://api.hello.com/users/$USER_ID_OR_NAME \
  -d '{
}' \
  -H "Content-Type: application/json"
```


#### Response Example

```
HTTP/1.1 200 OK
```

```json
{
  "created_at": "2015-01-01T12:00:00Z",
  "id": "01234567-89ab-cdef-0123-456789abcdef",
  "name": "example",
  "updated_at": "2015-01-01T12:00:00Z"
}
```

</details>


