# List Properties

**URL** : `/api/v1/properties/`

**Method** : `GET`

## Query Params

| Name  | Required | Description |
| ------------- | ------------- | ------------- |
| `limit`  | No  | |
| `offset`  | No  | |
| `agent`  | No  | Agent Id |
| `property_type`  | No  | Possible values: `Residential`, `Commercial`  |
| `property_subtype`  | No  | Possible values: `Condo`, `Land`, `House`, `House-Multi-Family`, `Condo-Multi-Family`, `Multi-Family`, `Other`, `Office`, `Industrial`, `Retail` |
| `status`  | No  | Possible values: `pending`, `active`, `uploading`, `inactive`, `sold` |

## Success Response

**Code** : `200 OK`

**Content examples**

```json
{
  "count": 1,
  "next": "http://127.0.0.1:8000/api/v1/properties/?limit=1&offset=1",
  "previous": null,
  "results": [
    {
      "id": 6,
      "location": {
        "lat": 12.0,
        "lng": 12.0
      },
      "agent": 2,
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
  ]
}
```
