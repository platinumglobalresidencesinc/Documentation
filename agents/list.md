# List Agents

**URL** : `/api/v1/agents/`

**Method** : `GET`

## Query Params

| Name  | Required | Description |
| ------------- | ------------- | ------------- |
| `limit`  | No  | |
| `offset`  | No  | |


## Success Response

**Code** : `200 OK`

**Content examples**

```json
{
    "count": 1,
    "next": "http://www.domain.com/api/v1/agents/?limit=1&offset=1",
    "previous": null,
    "results": [
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
    ]
}
```
