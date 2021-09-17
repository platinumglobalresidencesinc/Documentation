# Update Property Photo

**URL** : `/api/v1/property-photos/{id}/`

**Method** : `PUT`, `PATCH`

## Payload

* Content-Type: `multipart/form-data`, `json`

| Field  | Required | Example | Default Value | Description |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| `property`  | No  | |  | Property Id |
| `order`  | No  |  |  |  |


## Success Response

**Code** : `200 OK`

**Content examples**

```json
{
    "id": 2,
    "property": 2,
    "order": 3,
    "photo": "https://cloudfront_aws_cdn_domain/media/1/coding.jpg",
    "compressed_photo": "https://cloudfront_aws_cdn_domain/media/1/coding.jpg",
    "created_at": "2021-09-17T13:29:14.796302Z"
}
```

## Error Response

**Condition** : If provided data is invalid.

**Code** : `400 BAD REQUEST`

**Content example** :

```json
{
    "property": [
        "Error message"
    ],
    "order": [
        "Error message"
    ]
}
```
