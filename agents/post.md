# Create Agent

**URL** : `/api/v1/agents/`

**Method** : `POST`

## Payload

* Content-Type: `multipart/form-data`, `json`

| Field  | Required | Description | Default Value |
| ------------- | ------------- | ------------- | ------------- |
| `first_name`  | Yes  | |  |
| `last_name`  | Yes  | |  |
| `email`  | Yes  | |  |
| `country`  | Yes  | |  |
| `region`  | Yes  | |  |
| `city`  | Yes  | |  |
| `zip`  | Yes  | |  |
| `description`  | Yes  | |  |
| `description_language`  | Yes  | Possible values: `en`, `man`, `zh`, `he`, `ru`, `hi`, `de`, `it`, `es`, `nl`, `id`, `no`, `da`, `fi`, `el`, `pl`, `uk`, `ms`, `ar`, `ko`, `fr` |  |
| `able_to_login`  | No  | If `true`, system will create user for this agent, and he will be able to get password via forgot password option and manage assigned to him properties. | `false` |
| `agent_name`  | No  | | `null` |
| `phone`  | No  | | `null` |
| `mobile`  | No  | | `null` |
| `fax`  | No  | | `null` |
| `photo`  | No  | File  | `null` |
| `address`  | No  | | `null` |
| `url`  | No  | | `null` |
| `website`  | No  | | `null` |
| `linkedin_url`  | No  | | `null` |
| `facebook_url`  | No  | | `null` |
| `twitter_url`  | No  | | `null` |
| `instagram_url`  | No  | | `null` |
| `pinterest_url`  | No  | | `null` |
| `youtube_url`  | No  | | `null` |
| `native_language`  | No  | Possible values: `en`, `man`, `zh`, `he`, `ru`, `hi`, `de`, `it`, `es`, `nl`, `id`, `no`, `da`, `fi`, `el`, `pl`, `uk`, `ms`, `ar`, `ko`, `fr` | `null` |
| `agent_video_link`  | No  | | `null` |


## Success Response

**Code** : `201 CREATED`

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

## Error Response

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
