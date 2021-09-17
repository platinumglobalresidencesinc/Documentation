# Get Property Photo

**URL** : `/api/v1/property-photos/{id}/`

**Method** : `GET`

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

## Error Response: 404

**Condition** : If property photo doesn't exist.

**Code** : `404 NOT FOUND`
