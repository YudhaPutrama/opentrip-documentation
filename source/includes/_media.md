# Media

## Upload Photo Profile
> Success Result

```json
{
    "error":false,
    "data": {
        
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
    "location": "https://s3-ap-southeast-1.amazonaws.com/opentrip-media/592face38c13ad294405668bdd6488f85bae3381.jpg"
  }
}
```
### Endpoint

``POST /media/upload/cover``

### Query Parameters

Parameter | Required | Description
--------- | ------- | -----------
file | true | file of the image

## Upload Photo Activity
> Result

```json
{
  "error": false,
  "data": {
    "location": "https://s3-ap-southeast-1.amazonaws.com/opentrip-media/592face38c13ad294405668bdd6488f85bae3381.jpg"
  }
}
```
### Endpoint

``POST /media/upload/cover``

### Query Parameters

Parameter | Required | Description
--------- | ------- | -----------
file | true | file of the image

## Upload Video Cover
> Result

```json
{
  "error": false,
  "data": {
    "location": "https://s3-ap-southeast-1.amazonaws.com/opentrip-media/592face38c13ad294405668bdd6488f85bae3381.mp4"
  }
}
```
### Endpoint

``POST /media/upload/cover``

### Query Parameters

Parameter | Required | Description
--------- | ------- | -----------
file | true | file of the image
