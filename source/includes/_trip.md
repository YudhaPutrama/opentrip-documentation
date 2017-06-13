# Trip

<aside class="success">
Remember — a happy kitten is an authenticated kitten!
</aside>

## Create Trip
> Success Result

```json
{
    "error": false,
    "data": [
        {
            "_author": "5933658b705c0a671c510acd",
            "_category": "test",
            "main_image": "https:///tes",
            "title": "tes",
            "description": "ttt",
            "additional_note": "this is additional note",
            "important_notice": "eh ini important notice",
            "is_public": false,
            "quota": 5,
            "price": 40000,
            "_id": "593e7da24d5c58aa6c349d3a",
            "activities": [
                {
                    "title": "tess",
                    "image": "ini gambar",
                    "_id": "593e7da24d5c58aa6c349d3b",
                    "hourly": [
                        {
                            "start": 7,
                            "end": 8,
                            "activity": "makan-makan",
                            "_id": "593e7da24d5c58aa6c349d3c"
                        },
                        .....
                        .....
                        .....
                    ]
                },
                .....
                .....
                .....
            ],
            "date": {
                "start": "1970-01-18T07:54:10.267Z",
                "end": "1970-01-18T07:54:10.267Z"
            },
            "meeting_point": {
                "name": "name destination",
                "lat": -6.9739024,
                "long": 107.627451
            }
        },
        .....
        .....
        .....
        .....
    ]
}
```

creating new trip.

### Endpoint

`POST /trip/create`

<aside class="notice">
Remember — User must be verified to make trip
</aside>

<aside class="notice">
Use JSON body request
</aside>

### Body request
name | Required | Description
--------- | ------- | -----------
category | true | trip category
main_image | true | main header image
title | true | trip title
description | true | trip description
destination | true | trip destination
meeting_point | true | where meeting point
date | true | time to trip,use unix timestamp
is_public | true | is trip public
quota | true | trip quota
price | true | trip prize
price_included | true | price included
price_excluded | true | price excluded
activities | true | trip activities
requirement_equipment | true | price excluded
additional_note | false | additional note
important_notice | false | important notice


`see example request`


>Example Body Request

```json
{
	"category":"test",
	"main_image":"https:///tes",
	"title":"tes",
	"description":"ttt",
	"destination":{
		"name":"name destination",
		"lat":-6.9739024,
		"long":107.627451
	},
	"meeting_point":{
		"name":"name destination",
		"lat":-6.9739024,
		"long":107.627451
	},
	"date":[
		{
			"start":1497250267,
			"end":1497250267
		},
		{
			"start":1497250267,
			"end":1497250267
		}
	],
	"is_public":false,
	"quota":5,
	"price":40000,
	"price_included":"aaa,aaa,aa,",
	"price_excluded": "bbb,bbb,bbb,",
	"activities":[
		{
			"title":"tess",
			"image":"ini gambar",
			"hourly":[
				{
					"start":"07.00",
					"end": "08.00",
					"activity": "makan-makan"
				}
			]
		}
	],
	"requirement_equipment":"halah",
	"additional_note":"this is additional note",
	"important_notice":"eh ini important notice"
}
```





