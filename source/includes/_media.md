# Media

## Get Credential
> Success Result

```json
{
    "error":false,
    "data": {
        "endpoint_url":"https://opentrip-test-1.s3.amazonaws.com",
        "params": {
            "key":"26d585dd7047154130c0ce13af18dfa8.png",
            "acl":"public-read",
            "success_action_status":"201",
            "policy":"eyJleHBpcmF0aW9uIjoiMjAxNy0wNS0yNFQwNDoyMzoxOS43MTBaIiwiY29uZGl0aW9ucyI6W3siYnVja2V0IjoiYnJvd3Nlci11cGxvYWQtZGVtbyJ9LHsia2V5IjoiMjZkNTg1ZGQ3MDQ3MTU0MTMwYzBjZTEzYWYxOGRmYTgucG5nIn0seyJhY2wiOiJwdWJsaWMtcmVhZCJ9LHsic3VjY2Vzc19hY3Rpb25fc3RhdHVzIjoiMjAxIn0sWyJzdGFydHMtd2l0aCIsIiRDb250ZW50LVR5cGUiLCIiXSxbImNvbnRlbnQtbGVuZ3RoLXJhbmdlIiwwLDEwMDBdLHsieC1hbXotYWxnb3JpdGhtIjoiQVdTNC1ITUFDLVNIQTI1NiJ9LHsieC1hbXotY3JlZGVudGlhbCI6IkFLSUFKTTNOUVFLTzNSUldXM1hBLzIwMTcwNTI0L3VzLWVhc3QtMS9zMy9hd3M0X3JlcXVlc3QifSx7IngtYW16LWRhdGUiOiIyMDE3MDUyNFQwMDAwMDBaIn1dfQ==",
            "content-type":"image/png",
            "x-amz-algorithm":"AWS4-HMAC-SHA256",
            "x-amz-credential":"AKIAJM3NQQKO3RRWW3XA/20170524/us-east-1/s3/aws4_request",
            "x-amz-date":"20170524T000000Z",
            "x-amz-signature":"347fd27b055767e9a4fca7351a4739472025d013b2cf187a2ffa67f4226dffed"
        }
    }
}
```
### Endpoint

`POST /media/get_credential`

### Query Parameters
Parameter | Required | Description
--------- | ------- | -----------
filename | true | name of file "foto.png"
content_type | true | type of file eg. "image/png"

## Upload Media
> Result

```xml
<?xml version="1.0" encoding="UTF-8"?>
<PostResponse>
    <Location>https://browser-upload-demo.s3.amazonaws.com/26d585dd7047154130c0ce13af18dfa8.png</Location>
    <Bucket>browser-upload-demo</Bucket>
    <Key>26d585dd7047154130c0ce13af18dfa8.png</Key><ETag>"1d24dacdeb40056ae67dc9916dad37c4"</ETag>
</PostResponse>
```
### Endpoint

`HOST <endpoint-url-from-credentrial>`

`POST /`

### Query Parameters

Parameter | Required | Description
--------- | ------- | -----------
file | true | name of file "foto.png"
key | true | 'key' from credentitial
acl | true | 'acl' from credential
policy | true | 'policy' from credentitial
content-type | true | 'content-type' from credential
x-amz-algorithm | true | 'x-amz-algorithm' from credential
x-amz-credential | true | 'x-amz-credential' from credential
x-amz-date | true | 'x-amz-date' from credential
x-amz-signature | true | 'x-amz-signature' from credential