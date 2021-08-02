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
- `X-Session-Id` header


### Response
<details>
  <summary>Headers</summary>

  <br/>

  | Name             | Value                           |
  | ---------------- | ------------------------------- |
  | Content-Type     | application/json; charset=utf-8 |
  | X-Count          | 1                               |
  | X-Download-Token | bupvwse1                        |
  | X-Limit          | 1                               |
  | X-Offset         | 0                               |
  | X-Preview-Token  | 2e78f2ac                        |
  | Date             | Mon, 02 Aug 2021 12:47:38 GMT   |
  | Content-Length   | 1152                            |
</details>  

<details>
  <summary>JSON</summary>

  <br/>

  ```json
  [
   {
     "ID": "105",
     "UID": "pqx6gl7v6cl2xt4q",
     "Type": "video",
     "TypeSrc": "",
     "TakenAt": "2021-02-20T01:29:16Z",
     "TakenAtLocal": "2021-02-20T01:29:16Z",
     "TakenSrc": "",
     "TimeZone": "UTC",
     "Path": "videos",
     "Name": "20210220-012916-Not-A-Cat-2021",
     "OriginalName": "",
     "Title": "Not a Cat",
     "Description": "",
     "Year": 2021,
     "Month": 2,
     "Day": 20,
     "Country": "zz",
     "Stack": 0,
     "Favorite": false,
     "Private": false,
     "Iso": 0,
     "FocalLength": 0,
     "FNumber": 0,
     "Exposure": "",
     "Quality": 3,
     "Resolution": 0,
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
     "InstanceID": "",
     "FileUID": "fqx6gl831oq12wil",
     "FileRoot": "sidecar",
     "FileName": "videos/20210220-012916-Not-A-Cat-2021.mp4.jpg",
     "Hash": "cd78c8df6e40f522e71f160d063a947e7136292e",
     "Width": 480,
     "Height": 480,
     "Portrait": false,
     "Merged": false,
     "CreatedAt": "2021-08-01T20:22:19Z",
     "UpdatedAt": "2021-08-01T20:22:20Z",
     "EditedAt": "0001-01-01T00:00:00Z",
     "CheckedAt": "2021-08-01T20:31:50Z",
     "DeletedAt": "0001-01-01T00:00:00Z",
     "Files": null
   }
  ]
  ```
</details>  