# Update Agents

**URL** : `/api/v1/agents/{id}/`

**Method** : `PUT`, `PATCH`

## Payload

* Content-Type: `multipart/form-data`, `json`

| Field  |Description | Default Value |
| ------------- | ------------- | ------------- |
| `first_name`  | |  |
| `last_name`  | |  |
| `email`  | |  |
| `country`  | |  |
| `region`  | |  |
| `city`  | |  |
| `zip`  |  |  |
| `description`  | |  |
| `description_language`  | Possible values: `en`, `man`, `zh`, `he`, `ru`, `hi`, `de`, `it`, `es`, `nl`, `id`, `no`, `da`, `fi`, `el`, `pl`, `uk`, `ms`, `ar`, `ko`, `fr` |  |
| `able_to_login`  | | `false` |
| `agent_name`  | | `null` |
| `phone`  | | `null` |
| `mobile`  | | `null` |
| `fax`  | | `null` |
| `photo`  | File  | `null` |
| `address`  | | `null` |
| `url`  | | `null` |
| `website`  | | `null` |
| `linkedin_url`  | | `null` |
| `facebook_url`  | | `null` |
| `twitter_url`  | | `null` |
| `instagram_url`  | | `null` |
| `pinterest_url`  | | `null` |
| `youtube_url`  |  | `null` |
| `native_language`  | Possible values: `en`, `man`, `zh`, `he`, `ru`, `hi`, `de`, `it`, `es`, `nl`, `id`, `no`, `da`, `fi`, `el`, `pl`, `uk`, `ms`, `ar`, `ko`, `fr` | `null` |
| `agent_video_link`  | | `null` |


## Success Response

**Code** : `200 OK`

**Content examples**

```json
{
    "id": 100,
    "first_name": "test",
    "last_name": "alex",
    "agent_name": "test",
    "phone": "+XXXXXXXXXXXXXXXX",
    "mobile": "+XXXXXXXXXXXXXXXX",
    "fax": "+XXXXXXXXXXXXXXXX",
    "email": "test@test.com",
    "photo": "http://www.domain.com/image.jpg",
    "country": "United States",
    "region": "California",
    "city": "Los Angeles",
    "zip": "90001",
    "address": null,
    "url": null,
    "website": null,
    "linkedin_url": null,
    "facebook_url": null,
    "twitter_url": null,
    "instagram_url": null,
    "pinterest_url": null,
    "youtube_url": null,
    "description": "My description",
    "description_language": "en",
    "native_language": "en",
    "agent_video_link": null
}
```

## Error Response: 400

**Condition** : If provided data is invalid.

**Code** : `400 BAD REQUEST`

**Content example** :

```json
{
    "first_name": [
        "Error Message."
    ],
    "last_name": [
        "Error Message."
    ],
    "email": [
        "Error Message."
    ],
    "country": [
        "Error Message."
    ],
    "region": [
        "Error Message."
    ],
    "city": [
        "Error Message."
    ],
    "zip": [
        "Error Message."
    ],
    "description": [
        "Error Message."
    ],
    "description_language": [
        "Error Message."
    ]
}
```

## Error Response: 404

**Condition** : If agent doesn't exist.

**Code** : `404 NOT FOUND`

