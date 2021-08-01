# GET /api/v1/photos
Returns a list of photos and videos.

The table contains only main parameters. Full list of parameters can be found in [PhotoSearch struct](https://github.com/photoprism/photoprism/blob/ab40583c9a692730c57d4e9f5f1cd581daeed4c1/internal/form/photo_search.go#L8) implementation.

Useful links:
- [API handler implementation](https://github.com/photoprism/photoprism/blob/ab40583c9a692730c57d4e9f5f1cd581daeed4c1/internal/api/photo_search.go#L27)


| Parameter             | Type   | Description                                                                                              |
| --------------------- | ------ | -------------------------------------------------------------------------------------------------------- |
| q                     | String | Query string. Can be any search string. Supports special format: [param1]:[value1] [param2]:[value2] ... |
| label                 | String | Label (see get-labels)                                                                                   |
| cat                   | String | Category                                                                                                 |
| country               | String | Country code (format: "ru")                                                                              |
| camera                | Int    | Camera ID (0 - all, 1-...)                                                                               |
| order                 | String | Sort order (see [sorting values](../sorting-values.md))                                                  |
| count <br> (required) | Int    | Max result count                                                                                         |
| offset                | Int    | Result offset                                                                                            |
| before                | Date   | Find photos taken before (format: "2006-01-02")                                                          |
| after                 | Date   | Find photos taken after (format: "2006-01-02")                                                           |
| favorite              | Bool   | Find favorites only                                                                                      |
| merged                | Bool   | Find merged photos only (dublicates)                                                                     |
| year                  | Int    | Year number (format: YYYY)                                                                               |
| month                 | Int    | Month number (format: 1-12)                                                                              |
| day                   | Int    | Day number (format: 1-31?)                                                                               |
| video                 | Bool   | Find videos only                                                                                         |
| private               | Bool   | Find private only                                                                                        |
| public                | Bool   | Find public only                                                                                         |
| hidden                | Bool   | Find hidden only                                                                                         |
| archived              | Bool   | Find archived only                                                                                       |
| review                | Bool   | Find those that require review                                                                           |
| color                 | String | Find photos containing color (average color among whole photo or video preview )                         |
| album                 | String | Album UID                                                                                                |


# Example
Request: `/api/v1/photos?count=1`

Response:
```json
[
  {
    "ID": "130",
    "UID": "pqwujsr25o0r0mji",
    "Type": "image",
    "TypeSrc": "",
    "TakenAt": "2021-07-26T10:00:27Z",
    "TakenAtLocal": "2021-07-26T10:00:27Z",
    "TakenSrc": "",
    "TimeZone": "UTC",
    "Path": "2021/07",
    "Name": "20210726_100027_2B2F9E01",
    "OriginalName": "20160528_215318",
    "Title": "Unknown",
    "Description": "",
    "Year": -1,
    "Month": -1,
    "Day": -1,
    "Country": "zz",
    "Stack": 0,
    "Favorite": true,
    "Private": false,
    "Iso": 0,
    "FocalLength": 0,
    "FNumber": 0,
    "Exposure": "",
    "Quality": 5,
    "Resolution": 3,
    "Color": 0,
    "Scan": false,
    "Panorama": false,
    "CameraID": 1,
    "CameraModel": "Unknown",
    "CameraMake": "",
    "LensID": 1,
    "LensModel": "Unknown",
    "LensMake": "",
    "Lat": 0,
    "Lng": 0,
    "CellID": "zz",
    "PlaceID": "zz",
    "PlaceSrc": "",
    "PlaceLabel": "Unknown",
    "PlaceCity": "Unknown",
    "PlaceState": "Unknown",
    "PlaceCountry": "zz",
    "InstanceID": "0f4aff74-11c0-4f3e-b37e-9d1512799028",
    "FileUID": "fqwujss3rrp61qlg",
    "FileRoot": "/",
    "FileName": "2021/07/20210726_100027_2B2F9E01.jpg",
    "Hash": "047b661c271ebea1efe54ef5275f9cabd0eb101a",
    "Width": 1705,
    "Height": 1705,
    "Portrait": false,
    "Merged": false,
    "CreatedAt": "2021-07-26T10:00:27.836808257Z",
    "UpdatedAt": "2021-07-26T10:02:48.897720889Z",
    "EditedAt": "2021-07-26T10:02:49Z",
    "CheckedAt": "2021-07-26T10:15:43Z",
    "DeletedAt": "0001-01-01T00:00:00Z",
    "Files": null
  }
]
```