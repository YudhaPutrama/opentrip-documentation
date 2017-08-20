#Booking

##Get Order ID
> Success Result

```json
{
    "error": false,
    "data":{
        "booking_code":"OPIJDNK"
        "amount":"10000"
    }
}
```
get order id to (this is for mobile sdk)

### Endpoint

`POST /booking/get_payment_token`

### Query Parameters
Parameter | Required | Example/Description
--------- | ------- | -----------
trip_id   | true    | trip `_id`
joined_id |true |  `_joined_id` of field in date trip
promo_code| false | voucher code

<aside class="notice">
The time to make the payment process is 60 minutes until the order will be canceled.
time to process payment : 15 minute
time to complete payment : 45 minute
</aside>



##Get Payment Token
> Success Result

```json
{
    "error": false,
    "data":{
        "token":"easas-asdasd-asdasd",
        "booking_code":"OPIJDNK"
    }
}
```
get payament token to pay trip

### Endpoint

`POST /booking/get_payment_token`

### Query Parameters
Parameter | Required | Example/Description
--------- | ------- | -----------
trip_id   | true    | trip `_id`
joined_id |true |  `_joined_id` of field in date trip
promo_code| false | voucher code

<aside class="notice">
The time to make the payment process is 60 minutes until the order will be canceled.
time to process payment : 15 minute
time to complete payment : 45 minute
</aside>

##Cancel Booking
> Success Result

```json
{
    "error": false
}
```
to cancel booking, note this is cancel booking not cancel join trip
### Endpoint

`POST /booking/cancel`

### Query Parameters
Parameter | Required | Example/Description
--------- | ------- | -----------
booking_code| false | voucher code

