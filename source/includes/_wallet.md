#Wallet

## Wallet Balance
> Success Result

```json
{
    "error": false,
    "data":{
         "_author":"sadasdasda",
         "amount":0,
         "currency":"IDR"
    }
}
```
get user wallet balance

### Endpoint

`GET /wallet/balance`


## Wallet History
> Success Result

```json
{
    "error": false,
    "data":[
    {
         "_author":"sadasdasda",
         "action":"payment",
         "amount":20
         "initial_balance":0,
         "final_balance":20,
         "note":"OPS3434"
    },
    {
             "_author":"sadasdasda",
             "action":"refund",
             "amount":20
             "initial_balance":20,
             "final_balance":0,
             "note":"OPS3434"
    },
    {
             "_author":"sadasdasda",
             "action":"withdrawal",
             "amount":3000
             "initial_balance":4000,
             "final_balance":1000,
             "note":"OPS3434"
    },
    {
             "_author":"sadasdasda",
             "action":"transfer",
             "amount":3000
             "initial_balance":4000,
             "final_balance":1000,
             "note":"OPS3434"
     },
     {
              "_author":"sadasdasda",
              "action":"receive_transfer",
              "amount":3000
              "initial_balance":4000,
              "final_balance":1000,
              "note":"OPS3434"
      },
       {
                 "_author":"sadasdasda",
                 "action":"topup",
                 "amount":3000
                 "initial_balance":4000,
                 "final_balance":7000,
                 "note":"OPS3434"
        },
    ]
}
```
get user wallet history

### Endpoint

`GET /wallet/balance`

### Query Parameters
Parameter | Required | Example/Description
--------- | ------- | -----------
limit        | false    | limit get user data
offset         |false | start from offset
sort      |  false  | sorting
action | optional | "payment","refund","withdrawal","transfer","receive_transfer","topup"
from_date | optional | "2017-05-21"
to_date | optional | "2017-06-1"
