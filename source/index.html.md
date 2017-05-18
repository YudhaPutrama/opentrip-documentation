---
title: Open Trip API Reference

language_tabs:
  - json

toc_footers:
  - <a href='#'>Sign Up for a Developer Key</a>
  - <a href='https://github.com/tripit/slate'>Documentation Powered by Slate</a>

includes:
  - errors

search: true
---

# Introduction

Welcome to Open Trip API! Use `http://opentrip.trivalier.id` for endpoint host


# Authentication

Open Trip Authentication using JWT
`Authorization: Bearer <access_token>`

<aside class="notice">
You must replace <code>access-token</code> with access-token.
</aside>

# User

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

Register a new user using email

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

## Update User Profile

> Result

```json
{
    "error": false,
    "data": {
        "_id": "591a7f0278448125a40e2e05",
        "updatedAt": "2017-05-16T04:24:34.997Z",
        "createdAt": "2017-05-16T04:24:34.997Z",
        "name": "Kurniawan Yudha Putrama",
        "point": 0,
        "interest": [],
        "email": {
            "data": "kurniawan.yudha.p@gmail.com",
            "verified": false,
            "key": "YsiB178DsupgDWKKIFivQLWprbpMNmkReME"
        },
        "access_token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjU5MWE3ZjAyNzg0NDgxMjVhNDBlMmUwNSIsInR5cGUiOiJhY2Nlc3NfdG9rZW4iLCJpYXQiOjE0OTUwODA4NzIsImV4cCI6MTUwMDI2NDg3Mn0.ifqk3SbJClaXMTQ0Xi9O8uZpCZgt348JfByppTy5lBQ",
        "refresh_token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjU5MWE3ZjAyNzg0NDgxMjVhNDBlMmUwNSIsInR5cGUiOiJyZWZyZXNoX3Rva2VuIiwiaWF0IjoxNDk1MDgwODcyLCJleHAiOjE1MjY2Mzg0NzJ9.sPfngp5sGdih8mzx0VZdlDMQwcDutw0IWMC6yhMQuug"
    }
}
```

This endpoint retrieves a specific kitten.

<aside class="warning">Inside HTML code blocks like this one, you can't use Markdown, so use <code>&lt;code&gt;</code> blocks to denote code.</aside>

### Endpoint

`POST /user/login`

### Parameters

Parameter | Required | Description
--------- | ---------| -----------
email | true | Email for identifier
password | true | Password for identifier

## Forget Password

> Result

```json
{
    "error": false,
    "data": {
        "_id": "591a7f0278448125a40e2e05",
        "updatedAt": "2017-05-16T04:24:34.997Z",
        "createdAt": "2017-05-16T04:24:34.997Z",
        "name": "Kurniawan Yudha Putrama",
        "point": 0,
        "interest": [],
        "email": {
            "data": "kurniawan.yudha.p@gmail.com",
            "verified": false,
            "key": "YsiB178DsupgDWKKIFivQLWprbpMNmkReME"
        },
        "access_token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjU5MWE3ZjAyNzg0NDgxMjVhNDBlMmUwNSIsInR5cGUiOiJhY2Nlc3NfdG9rZW4iLCJpYXQiOjE0OTUwODA4NzIsImV4cCI6MTUwMDI2NDg3Mn0.ifqk3SbJClaXMTQ0Xi9O8uZpCZgt348JfByppTy5lBQ",
        "refresh_token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjU5MWE3ZjAyNzg0NDgxMjVhNDBlMmUwNSIsInR5cGUiOiJyZWZyZXNoX3Rva2VuIiwiaWF0IjoxNDk1MDgwODcyLCJleHAiOjE1MjY2Mzg0NzJ9.sPfngp5sGdih8mzx0VZdlDMQwcDutw0IWMC6yhMQuug"
    }
}
```

This endpoint retrieves a specific kitten.

<aside class="warning">Inside HTML code blocks like this one, you can't use Markdown, so use <code>&lt;code&gt;</code> blocks to denote code.</aside>

### Endpoint

`POST /user/login`

### Parameters

Parameter | Required | Description
--------- | ---------| -----------
email | true | Email for identifier
password | true | Password for identifier

