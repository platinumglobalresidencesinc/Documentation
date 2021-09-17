# Update Property

**URL** : `/api/v1/properties/{id}/`

**Method** : `PUT`, `PATCH`

## Payload

* Content-Type: `json`

| Field  | Required | Example | Default Value | Description |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| `agent`  | Yes  | |  | Agent Id |
| `location`  | Yes  | `{"lat": 71.1, "lng": 72.0}` |  |  |
| `property_type`  | Yes  | |  | Possible values: `Residential`, `Commercial` |
| `property_subtype`  | Yes  | |  | Possible values: `Condo`, `Land`, `House`, `House-Multi-Family`, `Condo-Multi-Family`, `Multi-Family`, `Other`, `Office`, `Industrial`, `Retail` |
| `status`  | Yes  | |  | Possible values: `pending`, `active`, `uploading`, `inactive`, `sold` |
| `price`  | Yes (if `price_min` and `price_max` empty)  | |  | Use only when specified `buy_rent` is `buy` |
| `price_min`  | Yes (if `price` empty)  | |  | Use only when specified `buy_rent` is `buy` |
| `price_max`  | Yes (if `price` empty)  | |  | Use only when specified `buy_rent` is `buy` |
| `monthly_hoa_fee`  | Yes (if `monthly_hoa_fee_min` and `monthly_hoa_fee_max` empty)  | |  | Use only when specified `buy_rent` is `rent` |
| `monthly_hoa_fee_min`  | Yes (if `monthly_hoa_fee` empty)  | |  | Use only when specified `buy_rent` is `rent` |
| `monthly_hoa_fee_max`  | Yes (if `monthly_hoa_fee` empty)  | |  | Use only when specified `buy_rent` is `rent` |
| `price_currency`  | No  | | `USD` | Accept currency code according to `ISO 4217` |
| `price_min_currency`  | No  | | `USD` | Accept currency code according to `ISO 4217` |
| `price_max_currency`  | No  | | `USD` | Accept currency code according to `ISO 4217` |
| `monthly_hoa_fee_currency`  | No  | | `USD` | Accept currency code according to `ISO 4217` |
| `monthly_hoa_fee_min_currency`  | No  | | `USD` | Accept currency code according to `ISO 4217` |
| `monthly_hoa_fee_max_currency`  | No  | | `USD` | Accept currency code according to `ISO 4217` |
| `address`  | Yes  | |  |  |
| `country`  | Yes  | |  |  |
| `region`  | Yes  | |  |  |
| `city`  | Yes  | |  |  |
| `district`  | No  | |  |  |
| `zip_code`  | Yes  | |  |  |
| `street`  | Yes  | |  |  |
| `beds`  | No  | |  |  |
| `beds_min`  | No  | |  |  |
| `beds_max`  | No  | |  |  |
| `baths`  | No  | |  |  |
| `baths_min`  | No  | |  |  |
| `baths_max`  | No  | |  |  |
| `size`  | No  | |  |  |
| `lot_size`  | No  | |  |  |
| `lot_size_min`  | No  | |  |  |
| `lot_size_max`  | No  | |  |  |
| `building_area`  | No  | |  |  |
| `parking_space`  | No  | |  |  |
| `build_year`  | No  | |  |  |
| `unit`  | No  | |  |  |
| `amenities`  | No  | |  |  |
| `description`  | Yes  | |  |  |
| `description_language`  | Yes  | |  | Possible values: `en`, `man`, `zh`, `he`, `ru`, `hi`, `de`, `it`, `es`, `nl`, `id`, `no`, `da`, `fi`, `el`, `pl`, `uk`, `ms`, `ar`, `ko`, `fr` |
| `buy_rent`  | Yes  | |  | Possible values: `buy`, `rent` |
| `grm`  | No  | |  |  |


## Success Response

**Code** : `200 OK`

**Content examples**

```json
{
    "id": 1,
    "location": {
        "lat": 12.0,
        "lng": 12.0
    },
    "agent": 1,
    "property_type": "Residential",
    "property_subtype": "Condo",
    "status": "active",
    "price": "100.00",
    "price_min": null,
    "price_max": null,
    "monthly_hoa_fee": null,
    "monthly_hoa_fee_min": null,
    "monthly_hoa_fee_max": null,
    "price_currency": "USD",
    "price_min_currency": "USD",
    "price_max_currency": "USD",
    "monthly_hoa_fee_currency": "USD",
    "monthly_hoa_fee_min_currency": "USD",
    "monthly_hoa_fee_max_currency": "USD",
    "address": "260-C North El Camino Real",
    "country": "United States",
    "region": "California",
    "city": "Encinitas",
    "district": "",
    "zip_code": "92024",
    "street": "North El Camino Real",
    "beds": null,
    "beds_min": "1.0",
    "beds_max": "2.0",
    "baths": null,
    "baths_min": "1.0",
    "baths_max": "2.0",
    "size": "100.00",
    "lot_size": null,
    "lot_size_min": "100.00",
    "lot_size_max": "200.00",
    "building_area": "200.00",
    "parking_space": "100.00",
    "build_year": 1999,
    "unit": null,
    "amenities": null,
    "description": "Beautifiul description",
    "description_language": "en",
    "buy_rent": "buy",
    "grm": null,
    "cap_rate": null,
    "website_link": null,
    "live_tour_link": null,
    "tenancy": null
}
```

## Error Response

**Condition** : If provided data is invalid.

**Code** : `400 BAD REQUEST`

**Content example** :

```json
{
    "location": [
        "Error message"
    ],
    "agent": [
        "Error message"
    ],
    "property_type": [
        "Error message"
    ],
    "property_subtype": [
        "Error message"
    ],
    "status": [
        "Error message"
    ],
    "address": [
        "Error message"
    ],
    "country": [
        "Error message"
    ],
    "region": [
        "Error message"
    ],
    "city": [
        "Error message"
    ],
    "zip_code": [
        "Error message"
    ],
    "street": [
        "Error message"
    ],
    "description": [
        "Error message"
    ],
    "description_language": [
        "Error message"
    ],
    "buy_rent": [
        "Error message"
    ]
}
```
## Error Response

**Condition** : If provided location data is invalid.

**Code** : `400 BAD REQUEST`

**Content example** :

```json
{
    "location": {
        "lat": "Invalid value.",
        "lng": "Invalid value."
    }
}
```

## Error Response: 404

**Condition** : If property doesn't exist.

**Code** : `404 NOT FOUND`

