# Profile

## Get User Profile

> Result

```json
{
  "error": false,
  "data": {
    "_id": "59239a99feb15e3830fd8813",
    "updatedAt": "2017-05-23T02:15:21.075Z",
    "createdAt": "2017-05-23T02:12:41.283Z",
    "name": "njayen",
    "address": "jalan jalan",
    "bio": "Gas",
    "birth_date": "1970-01-18T07:24:20.306Z",
    "profile_cover": "url alamat cover",
    "profile_picture": "url alamat cover",
    "point": 0,
    "interest": [
      "apaya",
      "ehh"
    ],
    "gender": "MALE",
    "block": 0,
    "following": 0,
    "phone_number": {
      "data": "08783666786",
      "verified": false
    },
    "email": {
      "data": "muhammadarizals1@gmail.com",
      "verified": false
    },
    "followers": 0,
    "follow_you":false
  }
}
```

Get user data profile by id

### Endpoint

`GET /user/profile`

### Query Parameters

Parameter | Required | Description
--------- | ------- | -----------
id | true | user id `_id`
from | optional | user id `_id`,to get follow you or not



## Update User Profile

> Result

```json
{
  "error": false,
  "data": {
    "_id": "59239a99feb15e3830fd8813",
    "updatedAt": "2017-05-23T02:47:28.727Z",
    "createdAt": "2017-05-23T02:12:41.283Z",
    "name": "njayen baru",
    "address": "jl sukarn hatta bandung",
    "bio": "Logi",
    "birth_date": "1970-01-18T07:24:20.306Z",
    "profile_cover": "cover bary",
    "profile_picture": "url alamat profile picture baru",
    "point": 0,
    "interest": [
      "apaya",
      "ehh"
    ],
    "gender": "FEMALE",
    "block": 0,
    "following": 0,
    "phone_number": {
      "data": "14045",
      "verified": false
    },
    "email": {
      "data": "muhammadarizals2@gmail.com",
      "verified": false
    },
    "followers": 0
  }
}
```

You can update user profile using this endpoint.

### Endpoint

`PUT /user/update`

### Header

Name | Required | Description | example
--------- | ---------| -----------| -------------
Authorization | true | access_token | `Authorization: Bearer <access_token>`

<aside class="notice">
You must replace <code>access_token</code> with access_token.
</aside>

### Query Parameters

Parameter | Required | Description | Type
--------- | ------- | -----------| -----------
email | optional | new user email address | email
birth_date | optional | new user birth date | TIMESTAMP
interest | optional | new user interest on | Array of String `["a","b","c"]`
gender | optional | new user gender | MALE/FEMALE/UNKNOWN
phone_number | optional | new user phone_number | phone numeber
name | optional | new user name | String
bio | optional | new user bio | String
address | optional | new user address | String
identity_card | optional | new user identity_card `ktp` | Url image adresss
profile_cover | optional | new user cover photo | Url image adresss
profile_picture | optional | new user profile photo | Url image adresss


<aside class="notice">
You can use `json` type on body request
</aside>

<aside class="notice">
When you updating phone number user will receive sms verification
</aside>