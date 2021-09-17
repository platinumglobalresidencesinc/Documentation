# List Property Photos

**URL** : `/api/v1/property-photos/`

**Method** : `GET`

## Query Params

| Name  | Required | Description |
| ------------- | ------------- | ------------- |
| `limit`  | No  | |
| `offset`  | No  | |
| `property`  | No  | |

## Success Response

**Code** : `200 OK`

**Content examples**

```json
{
    "count": 1,
    "next": null,
    "previous": null,
    "results": [
        {
            "id": 6,
            "property": 2,
            "order": 1,
            "photo": "https://cloudfront_aws_cdn_domain/media/2/coding.jpg",
            "compressed_photo": "https://cloudfront_aws_cdn_domain/media/2/coding.jpg",
            "created_at": "2021-09-17T13:29:41.519223Z"
        }
    ]
}
```
