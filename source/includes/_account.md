# Account

## Register

> Result

```json
{
  "error": false,
  "data": {
    "updatedAt": "2017-05-18T06:39:31.966Z",
    "createdAt": "2017-05-18T06:39:31.966Z",
    "name": "Kurniawan",
    "_id": "591d41a3f80b8827308b2526",
    "point": 0,
    "interest": [],
    "email": {
      "data": "kurniawan.yudha.p@gmail.com",
      "verified": false,
      "key": "z0PGSaBivm2Asjx7m0TmNFfc0Q53AtBC612"
    },
    "following": 0,
    "follower": 0,
    "access_token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjU5MWQ0MWEzZjgwYjg4MjczMDhiMjUyNiIsInR5cGUiOiJhY2Nlc3NfdG9rZW4iLCJpYXQiOjE0OTUwODk1NzEsImV4cCI6MTUwMDI3MzU3MX0.fzVtnufkH7dGn15uYO4ke_SDQ6Q3P0oD01oqZT6zOkk",
    "refresh_token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjU5MWQ0MWEzZjgwYjg4MjczMDhiMjUyNiIsInR5cGUiOiJyZWZyZXNoX3Rva2VuIiwiaWF0IjoxNDk1MDg5NTcyLCJleHAiOjE1MjY2NDcxNzJ9.wr2zGhorpsUGJ2br0pBjPDh3s8JTEp1CUe-d6VhLMM0"
  }
}
```

Register a new user using email adn password

### Endpoint

`POST /user/register`

### Query Parameters

Parameter | Required | Description
--------- | ------- | -----------
name | true | Fullname for new user
email | true | Email for new user
password | true | Password for new user

<aside class="success">
Remember — a happy kitten is an authenticated kitten!
</aside>

## Login Manual

> Result

```json
{
  "error": false,
  "data": {
    "_id": "5921e5246518bb29d8159771",
    "updatedAt": "2017-05-21T19:06:12.934Z",
    "createdAt": "2017-05-21T19:06:12.934Z",
    "name": "paijo",
    "point": 0,
    "interest": [],
    "block": [],
    "following": 0,
    "email": {
      "data": "tes@tes.com",
      "verified": false,
      "key": "k6SgNkzFAFfHuNFWPNMtPQj99IajdMhA1go79lVm"
    },
    "followers": 0,
    "access_token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjU5MjFlNTI0NjUxOGJiMjlkODE1OTc3MSIsInR5cGUiOiJhY2Nlc3NfdG9rZW4iLCJpYXQiOjE0OTU0MjUzODgsImV4cCI6MTUwMDYwOTM4OH0.8AP4seI3HOCiJqP-2QXzr46MzpNkPca80lm1crgdV7A",
    "refresh_token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjU5MjFlNTI0NjUxOGJiMjlkODE1OTc3MSIsInR5cGUiOiJyZWZyZXNoX3Rva2VuIiwiaWF0IjoxNDk1NDI1Mzg4LCJleHAiOjE1MjY5ODI5ODh9.CE2cKlVzuyzfduwl7OGC1JzzkRJni-ctPNn4ZhsqzV0"
  }
}
```

User login application with email and password.


### Endpoint

`POST /user/login`

### Parameters

Parameter | Required | Description
--------- | ---------| -----------
email | true | Email for identifier
password | true | Password for identifier

## Instagram Login

> Result

```json
{
  "error": false,
  "data": {
    "_id": "5921e5c4b9ffb22ac4b58e3c",
    "updatedAt": "2017-05-21T19:08:52.726Z",
    "createdAt": "2017-05-21T19:08:52.726Z",
    "name": "Arizal Saputro",
    "id_instagram": "1574083",
    "access_token_instagram": "fb2e77d.47a0479900504cb3ab4a1f626d174d2d",
    "profile_picture": "https://scontent-sin6-1.xx.fbcdn.net/v/t1.0-1/p160x160/11174930_992304550841336_4056769259860245295_n.jpg?oh=2f85c038be8336b14699cbbe7ac3f89b&oe=599F7276",
    "point": 0,
    "interest": [],
    "block": [],
    "following": 0,
    "followers": 0,
    "access_token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjU5MjFlNWM0YjlmZmIyMmFjNGI1OGUzYyIsInR5cGUiOiJhY2Nlc3NfdG9rZW4iLCJpYXQiOjE0OTU0MjU3MzQsImV4cCI6MTUwMDYwOTczNH0.PV5me3Ljcy4EYjVk4pkRx97jyvFGmHFpM502qk-6rGA",
    "refresh_token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjU5MjFlNWM0YjlmZmIyMmFjNGI1OGUzYyIsInR5cGUiOiJyZWZyZXNoX3Rva2VuIiwiaWF0IjoxNDk1NDI1NzM0LCJleHAiOjE1MjY5ODMzMzR9.r9KeRQ4Gp9mhb1Fk-DCpqfzgI4LmwM0lqFyOuwxltBE"
  }
}
```

User login application with instagram account.


### Endpoint

`POST /user/login_instagram`

### Parameters

Parameter | Required | Description
--------- | ---------| -----------
access_token | true | user access_token by instagram account
id | true | user id instagram account
username | true | username instagram account
profile_picture | false | user profile picture
full_name | false | user full_name of instagram account


## Forget Password

> Result

```json
{
    "error": false,
}
```

User will receive email to reset password


### Endpoint

`POST /user/forget_password`

### Parameters

Parameter | Required | Description
--------- | ---------| -----------
email | true | Registered email address

## Verify Email

> Result

```json
{
  "error": false,
  "data": {
    "updatedAt": "2017-05-22T04:27:23.049Z",
    "_id": "5921e5246518bb29d8159771",
    "email": {
      "data": "tes@tes.com",
      "verified": true
    }
  }
}
```

To verify user email address


### Endpoint

`PUT /user/confirm_email`

### Parameters

Parameter | Required | Description
--------- | ---------| -----------
key | true | Unique key from to verify email address

## RefreshToken

> Result

```json
{
  "error": false,
  "data": {
    "_id": "5921e5246518bb29d8159771",
    "access_token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjU5MjFlNTI0NjUxOGJiMjlkODE1OTc3MSIsInR5cGUiOiJhY2Nlc3NfdG9rZW4iLCJpYXQiOjE0OTU0Mjc4NDQsImV4cCI6MTUwMDYxMTg0NH0.BkdPTO-H2NnB-kWxxPTDLpclc9L7pa-h7TRAuCGLtUc",
    "refresh_token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjU5MjFlNTI0NjUxOGJiMjlkODE1OTc3MSIsInR5cGUiOiJyZWZyZXNoX3Rva2VuIiwiaWF0IjoxNDk1NDI3ODQ0LCJleHAiOjE1MjY5ODU0NDR9.CRzb1_c2d536-bn-QG0JaDze5fAdyAHIwDcDT29R2eM"
  }
}
```

Get user access_token, use this then access_token was expired

### Endpoint

`GET /user/refresh_token`

### Header

Name | Required | Description | example
--------- | ---------| -----------| -------------
Authorization | true | refresh_token | `Authorization: Bearer <refresh_token>`

<aside class="notice">
You must replace <code>refresh_token</code> with refresh_token.
Remember! header is <code>refresh_token</code> , NOT <code>access_token</code>
</aside>