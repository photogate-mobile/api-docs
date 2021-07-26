# GET /api/v1/photos
Returns a list of photos and videos.

The table contains only main parameters. Full list of parameters can be found in [PhotoSearch struct](https://github.com/photoprism/photoprism/blob/ab40583c9a692730c57d4e9f5f1cd581daeed4c1/internal/form/photo_search.go#L8) implementation.

Useful links:
- [API handler implementation](https://github.com/photoprism/photoprism/blob/ab40583c9a692730c57d4e9f5f1cd581daeed4c1/internal/api/photo_search.go#L27)
- [Search implementation](https://github.com/photoprism/photoprism/blob/ab40583c9a692730c57d4e9f5f1cd581daeed4c1/internal/query/photo_search.go) 


<table>
  <tbody>
    <tr>
      <th align="center">Parameter</th>
      <th align="center">Type</th>
      <th align="center">Description</th>
    </tr>
    <tr>
      <td>q</td>
      <td>String</td>
      <td>Query string (format: "[param1]:[value1] [param2]:[value2] ...")</td>
    </tr>
    <tr>
      <td>label</td>
      <td>String</td>
      <td>Label (see get-labels)</td>
    </tr>
    <tr>
      <td>cat</td>
      <td>String</td>
      <td>Category</td>
    </tr>
    <tr>
      <td>country</td>
      <td>String</td>
      <td>Country code (format: "ru")</td>
    </tr>
    <tr>
      <td>camera</td>
      <td>Int</td>
      <td>Camera ID (0 - all, 1-...)</td>
    </tr>
    <tr>
      <td>order</td>
      <td>String</td>
      <td>
        Sort order
        <ul>
          <li>newest (Newest first)</li>
          <li>edited (Recently edited)</li>
          <li>added (Recently added)</li>
          <li>oldest (Oldest first)</li>
          <li>name (Sort by file name)</li>
          <li>similar (Group by similarity)</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td>count <br> (required)</td>
      <td>Int</td>
      <td>Max result count</td>
    </tr>
    <tr>
      <td>offset</td>
      <td>Int</td>
      <td>Result offset</td>
    </tr>
    <tr>
      <td>before</td>
      <td>Date</td>
      <td>Find photos taken before (format: "2006-01-02")</td>
    </tr>
    <tr>
      <td>after</td>
      <td>Date</td>
      <td>Find photos taken after (format: "2006-01-02")</td>
    </tr>
    <tr>
      <td>favorite</td>
      <td>Bool</td>
      <td>Find favorites only</td>
    </tr>
    <tr>
      <td>merged</td>
      <td>Bool</td>
      <td>Find merged photos only (dublicates)</td>
    </tr>
    <tr>
      <td>year</td>
      <td>Int</td>
      <td>Year number (format: YYYY)</td>
    </tr>
    <tr>
      <td>month</td>
      <td>Int</td>
      <td>Month number (format: 1-12)</td>
    </tr>
    <tr>
      <td>day</td>
      <td>Int</td>
      <td>Day number (format: 1-31?)</td>
    </tr>
    <tr>
      <td>video</td>
      <td>Bool</td>
      <td>Find videos only</td>
    </tr>
    <tr>
      <td>private</td>
      <td>Bool</td>
      <td>Find private only</td>
    </tr>
    <tr>
      <td>public</td>
      <td>Bool</td>
      <td>Find public only</td>
    </tr>
    <tr>
      <td>hidden</td>
      <td>Bool</td>
      <td>Find hidden only</td>
    </tr>
    <tr>
      <td>archived</td>
      <td>Bool</td>
      <td>Find archived only</td>
    </tr>
    <tr>
      <td>review</td>
      <td>Bool</td>
      <td>Find those that require review</td>
    </tr>
    <tr>
      <td>color</td>
      <td>String</td>
      <td>
        Find photos containing color (purple, magenta, pink, red, orange, gold, yellow, lime, green, teal, cyan, blue, brown, white, gray, black)
      </td>
    </tr>
    <tr>
      <td>album</td>
      <td>String</td>
      <td>Album UID</td>
    </tr>
  </tbody>
</table> 


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