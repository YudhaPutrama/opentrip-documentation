# Media

<aside class="success">
Remember — a happy kitten is an authenticated kitten!
</aside>

## Upload Photo Profile
> Success Result

```json
{
  "error": false,
  "data": {
    "updatedAt": "2017-06-04T02:04:59.575Z",
    "_id": "5933658b705c0a671c510acd",
    "profile_picture": "https://s3-ap-southeast-1.amazonaws.com/opentrip-media/5933658b705c0a671c510acd4ab69878b7e6c88f.jpg"
  }
}
```
### Endpoint

`POST /media/upload/profile`

### Query Parameters
Parameter | Required | Description
--------- | ------- | -----------
file | true | file of the image

## Upload Photo Cover
> Result

```json
{
  "error": false,
  "data": {
    "updatedAt": "2017-06-04T02:04:59.575Z",
    "_id": "5933658b705c0a671c510acd",
    "profile_cover": "https://s3-ap-southeast-1.amazonaws.com/opentrip-media/5933658b705c0a671c510acd4ab69878b7e6c88f.jpg"
  }
}
```
### Endpoint

``POST /media/upload/cover``

### Query Parameters

Parameter | Required | Description
--------- | ------- | -----------
file | true | file of the image

## Upload Image
> Success Result

```json
{
  "error": false,
  "data": {
    "location": "https://s3-ap-southeast-1.amazonaws.com/opentrip-media/5933658b705c0a671c510acd_b33c20a2b602ecf6.jpg"
  }
}
```

create/upload image.

### Endpoint

`POST /media/upload/image`

### Query Parameters
Parameter | Required | Description
--------- | ------- | -----------
file | true | file of the image

## Delete Image
> Success Result

```json
{
  "error": false
}
```

remove/delete image.

### Endpoint

`DELETE /media/upload/image`

### Query Parameters
Parameter | Required | Description
--------- | ------- | -----------
filename | true | url image



## Delete Photo Profile
> Success Result

```json
{
  "error": false,
  "data": {
    "_id": "5933658b705c0a671c510acd"
  }
}
```
### Endpoint

`DELETE /media/delete/profile`

## Delete Profile Cover
> Success Result

```json
{
  "error": false,
  "data": {
    "_id": "5933658b705c0a671c510acd"
  }
}
```
### Endpoint

`DELETE /media/delete/cover`
