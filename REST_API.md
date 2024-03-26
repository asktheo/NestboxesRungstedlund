
# REST API
Prefix methods below with http://server/context

## Nest boxes

GET
/nestbox: all nestboxes - properties only

Params:

- boxId: filter the list of nestboxes by property boxId

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

Params :

- boxId : filter list by property boxId

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


