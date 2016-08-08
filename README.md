# Indian Railways Data

This repository has Indian Railways data that [Sanjay](https://twitter.com/sanjaybhangar) and [Sajjad](https://twitter.com/geohacker) have been gathering for a few months. Read [more here]( http://sajjad.in/2016/08/gathering-indian-railways-data/). 

There are three JSON files:

### Stations
[GeoJSON](http://geojson.org/) FeatureCollection, each Feature is a Station and looks like:

```json
{
    "geometry": {
        "type": "Point",
        "coordinates": [75.4516454, 27.2520587]
    },
    "type": "Feature",
    "properties": {
        "state": "Rajasthan",
        "code": "BDHL",
        "name": "Badhal",
        "zone": "NWR",
        "address": "Kishangarh Renwal, Rajasthan"
    }
}
```

### Trains
GeoJSON FeatureCollection, each Feature is a Train and looks like:

```json
{
    "geometry": {
        "type": "LineString",
        "coordinates": [
            [72.89173899999999, 19.070320000000002],
            [78.2266994458, 26.0352337224],
            [78.18700399999999, 26.145594],
            [78.18229199999999, 26.216483]
        ]
    },
    "type": "Feature",
    "properties": {
        "third_ac": true,
        "arrival": "15:35:00",
        "from_station_code": "LTT",
        "name": "Mumbai LTT - Gwalior (Weekly) Special",
        "zone": "CR",
        "chair_car": true,
        "first_class": true,
        "duration_m": 45,
        "sleeper": true,
        "from_station_name": "LOKMANYA TILAK TERM",
        "number": "01101",
        "departure": "15:50:00",
        "return_train": "01102",
        "to_station_code": "GWL",
        "second_ac": true,
        "classes": "",
        "to_station_name": "GWALIOR JN",
        "duration_h": 23,
        "type": "Exp",
        "first_ac": true,
        "distance": 1216
    }
}
```

### Schedules
An array of objects. Each object is a schedule which defines a Train stop at a Station. 

```json
{
    "arrival": "None",
    "day": 1,
    "train_name": "Falaknuma Lingampalli MMTS",
    "station_name": "KACHEGUDA FALAKNUMA",
    "station_code": "FM",
    "id": 302214,
    "train_number": "47154",
    "departure": "07:55:00"
}
```

#### License

[CC0](https://wiki.creativecommons.org/wiki/CC0)

