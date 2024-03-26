
# REST API
Prefix methods below with http://server/context

## Nest boxes

GET
/nestbox: all nestboxes - properties only

QueryParams (not required):

- boxId: filter the result by property _boxId_
- altitude: filter the result by property _altitude_
- boxId: filter the result by property _boxId_

Return type : Array

Example output :

    [
      {
        "fid":88,
        "altitude":1,
        "boxId":"100",
        "zone":"48"
    }]

## Nest box features

GET
/nestbox/feature : all nestboxes as GeoJson features with properties 

Queryparams (not required):

- boxId : filter list by property _boxId_
- altitude : filter list by property _altitude_
- zone : filter liste by property _zone_

Return type: Array

Example output:

    [
      {
        "_id": {
          "timestamp": 1711326429,
          "date": "2024-03-25T00:27:09.000+00:00"
        },
        "properties": {
          "fid": 88,
          "altitude": 1,
          "boxId": "100",
          "zone": "48"
        },
        "geometry": {
          "type": "Point",
          "coordinates": [12.5412010720627, 55.8848459278126]
        },
        "type": "Feature"
      }
    ]

GET
/nestbox/feature/{fid} : the nestbox with unique id _fid_

Return type: Object {}

Example output:

    {
      "_id": {
        "timestamp": 1711485932,
        "date": "2024-03-26T20:45:32.000+00:00"
    },
      "properties": {
        "fid": 108,
        "altitude": 1,
        "boxId": "301",
        "zone": "13"
    },
      "geometry": {
        "type": "Point",
        "coordinates": [12.5416995606844, 55.8830301305001]
    },
      "type": "Feature"
    }


