# Get Agent

**URL** : `/api/v1/agents/{id}/`

**Method** : `GET`

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

## Error Response: 404

**Condition** : If agent doesn't exist.

**Code** : `404 NOT FOUND`
