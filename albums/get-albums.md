# GET /api/v1/albums
Returns a list of albums.

The table contains only main parameters. Full list of parameters can be found in [AlbumSearch struct](https://github.com/photoprism/photoprism/blob/5076af2979638b1722003ad6c22a0d59e4af76cf/internal/form/album_search.go#L4) implementation.

Useful links:
- [API handler implementation](https://github.com/photoprism/photoprism/blob/5076af297963/internal/api/album.go#L44)


| Parameter             | Type   | Description                                                                                              |
| --------------------- | ------ | -------------------------------------------------------------------------------------------------------- |
| q                     | String | Query string. Can be any search string. Supports special format: [param1]:[value1] [param2]:[value2] ... |
| id                    | String | Album UID                                                                                                |
| type                  | String | Album type (album, moment, folder, state)                                                                |
| title                 | String | Find albums by their title                                                                               |
| country               | String | Country code (format: "ru")                                                                              |
| year                  | Int    | Year number (format: YYYY)                                                                               |
| month                 | Int    | Month number (format: 1-12)                                                                              |
| day                   | Int    | Day number (format: 1-31?)                                                                               |
| favorite              | Bool   | Find favorites only                                                                                      |
| private               | Bool   | Find private only                                                                                        |
| count <br> (required) | Int    | Max result count                                                                                         |
| offset                | Int    | Result offset                                                                                            |
| order                 | String | Sort order (see [sorting values](../sorting-values.md))                                                  |


# Example
Request: `/api/v1/albums?count=1`

Response:
```json
[
  {
    "UID": "aqx6gl9351sd0u1a",
    "CoverUID": "",
    "FolderUID": "",
    "Slug": "february-2021",
    "Type": "month",
    "Title": "February 2021",
    "Location": "",
    "Category": "",
    "Caption": "",
    "Description": "",
    "Notes": "",
    "Filter": "public:true year:2021 month:2",
    "Order": "oldest",
    "Template": "",
    "Path": "",
    "Country": "zz",
    "Year": 2021,
    "Month": 2,
    "Day": 0,
    "Favorite": false,
    "Private": false,
    "PhotoCount": 0,
    "LinkCount": 0,
    "CreatedAt": "2021-08-01T20:22:22Z",
    "UpdatedAt": "2021-08-01T20:22:22Z",
    "DeletedAt": "0001-01-01T00:00:00Z"
  }
]
```