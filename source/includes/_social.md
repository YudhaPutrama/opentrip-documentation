# Social

## Get User Following

> Result

```json
{
  "error": false,
  "data": [
    {
      "_id": "5923cfc450434044b836c3b8",
      "profile_picture": "image url profile picture",
      "name": "arizal"
    },
    {
      "_id": "592510f6f856d02284b2f44b",
      "profile_picture": "image url profile picture"
      "name": "bibibi testititititi"
    },
    {
      "_id": "59251006f856d02284b2f44a",
      "profile_picture": "image url profile picture"
      "name": "testititititi"
    }
  ]
}
```

Get user data following by id

### Endpoint

`GET /user/social/following`

### Query Parameters

Parameter | Required |  Type     | Description
--------- | ------- | -----------| --------
id | true | id | user id `_id`
limit | optional | number | how much data
offset | optional | number | from where

<aside class="notice">
default limit : <code>15</code> offset : <code>0</code>
</aside>


## Get User Followers

> Result

```json
{
  "error": false,
  "data": [
    {
      "_id": "5923cfc450434044b836c3b8",
      "profile_picture": "image url profile picture",
      "name": "arizal"
    },
    {
      "_id": "592510f6f856d02284b2f44b",
      "profile_picture": "image url profile picture"
      "name": "bibibi testititititi"
    },
    {
      "_id": "59251006f856d02284b2f44a",
      "profile_picture": "image url profile picture"
      "name": "testititititi"
    }
  ]
}
```

Get user data followers by id

### Endpoint

`GET /user/social/followers`

### Query Parameters

Parameter | Required |  Type     | Description
--------- | ------- | -----------| --------
id | true | id | user id `_id`
limit | optional | number | how much data
offset | optional | number | from where

<aside class="notice">
default `limit : <code>15</code> offset : <code>0</code>
</aside>


## Get User Blocked

> Result

```json
{
  "error": false,
  "data": [
    {
      "_id": "5923cfc450434044b836c3b8",
      "profile_picture": "image url profile picture",
      "name": "arizal"
    },
    {
      "_id": "592510f6f856d02284b2f44b",
      "profile_picture": "image url profile picture"
      "name": "bibibi testititititi"
    },
    {
      "_id": "59251006f856d02284b2f44a",
      "profile_picture": "image url profile picture"
      "name": "testititititi"
    }
  ]
}
```

Get user data following by id

### Endpoint

`GET /user/social/blocked`

### Header

Name | Required | Description | example
--------- | ---------| -----------| -------------
Authorization | true | access_token | `Authorization: Bearer <access_token>`

<aside class="notice">
You must replace <code>access_token</code> with access_token.
</aside>


### Query Parameters

Parameter | Required |  Type     | Description
--------- | ------- | -----------| --------
limit | optional | number | how much data
offset | optional | number | from where

<aside class="notice">
default limit : <code>15</code> offset : <code>0</code>
</aside>



## Action Follow

> Result

```json
{
  "error": false
}
```
You can follow another user profile using this endpoint.

### Endpoint

`POST /user/social/action/follow`

### Header

Name | Required | Description | example
--------- | ---------| -----------| -------------
Authorization | true | access_token | `Authorization: Bearer <access_token>`

<aside class="notice">
You must replace <code>access_token</code> with access_token.
</aside>


### Query Parameters

Parameter | Required | Description
--------- | ------- | --------
id | true | another user id to follow

## Action Unfollow

> Result

```json
{
  "error": false
}
```
You can unfollow another user profile using this endpoint.

### Endpoint

`POST /user/social/action/unfollow`

### Header

Name | Required | Description | example
--------- | ---------| -----------| -------------
Authorization | true | access_token | `Authorization: Bearer <access_token>`

<aside class="notice">
You must replace <code>access_token</code> with access_token.
</aside>

### Query Parameters

Parameter | Required | Description
--------- | ------- | --------
id | true | another user id to unfollow

## Action Block

> Result

```json
{
  "error": false
}
```
You can block another user profile using this endpoint.

### Endpoint

`POST /user/social/action/block`

### Header

Name | Required | Description | example
--------- | ---------| -----------| -------------
Authorization | true | access_token | `Authorization: Bearer <access_token>`

<aside class="notice">
You must replace <code>access_token</code> with access_token.
</aside>

### Query Parameters

Parameter | Required | Description
--------- | ------- | --------
id | true | another user id to block

## Action Unblock

> Result

```json
{
  "error": false
}
```
You can block another user profile using this endpoint.

### Endpoint

`POST /user/social/action/unblock`

### Header

Name | Required | Description | example
--------- | ---------| -----------| -------------
Authorization | true | access_token | `Authorization: Bearer <access_token>`

<aside class="notice">
You must replace <code>access_token</code> with access_token.
</aside>

### Query Parameters

Parameter | Required | Description
--------- | ------- | --------
id | true | another user id to unblock
