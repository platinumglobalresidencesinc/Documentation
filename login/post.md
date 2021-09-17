# Obtain API Token

**URL** : `/api/v1/login/`

**Method** : `POST`

**Permissions** : You should have access to API in other way you will get 403.

## Payload

* Content-Type: `multipart/form-data`, `json`

| Field  | Required |
| ------------- | ------------- |
| `username`  | Yes  |
| `password`  | Yes  |

## Success Response

**Code** : `200 OK`

**Content examples**

```json
{
    "token": "11111111-043d-4c95-ba77-d7b9f248d21e"
}
```

## Error Response 

### 400 Bad Request

**Condition** : Invalid credentials.

**Code** : `400 Bad Request`

### 403 Forbidden

**Condition** : You don't have access to API.

**Code** : `403 Forbidden`
