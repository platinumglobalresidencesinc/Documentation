![MLSWorldWide Logo](https://ci5.googleusercontent.com/proxy/OSca2ixc5IjnouIi-gjP34tKEMHMQ2z0xV3w2tlSNOgxazvHuoWUD-AuB3eiIlr5HaR7bs-JQW8=s0-d-e1-ft#https://mlsworldwide.com/mls-logo.png)

# API Documentation

| API Domain Name |
| ------------- |
| https://admin.mlsworldwide.com  |

##Auth Headers
| Header Name  | Value |
| ------------- | ------------- |
| `Authorization`  | `Token  xxxxxxxxxxxxxxxx`  |

##Pagination
For some API methods you will get paginated response,
it's used simple limit offset pagination. Max result is 100 items per page.

## Authentication API

* [Obtain API Token](login/post.md) : `POST /api/v1/login/`

## Agents API

* [List Agents](agents/list.md) : `GET /api/v1/agents/`
* [Create Agent](agents/post.md) : `POST /api/v1/agents/`
* [Get Agent](agents/get.md) : `GET /api/v1/agents/{id}/`
* [Update Agent](agents/put.md) : `PUT /api/v1/agents/{id}/`
* [Delete Agent](agents/delete.md) : `DELETE /api/v1/agents/{id}/`


## Properties API

* [List Properties](properties/list.md) : `GET /api/v1/properties/`
* [Create Property](properties/post.md) : `POST /api/v1/properties/`
* [Get Property](properties/get.md) : `GET /api/v1/properties/{id}/`
* [Update Property](properties/put.md) : `PUT /api/v1/properties/{id}/`
* [Delete Property](properties/delete.md) : `DELETE /api/v1/properties/{id}/`

## Properties Photos API
