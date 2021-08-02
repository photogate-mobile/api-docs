# GET /api/v1/photos/:uid
Returns full information about photo (video). 

Useful links:
- [API handler implementation](https://github.com/photoprism/photoprism/blob/5076af297963/internal/api/photo.go#L42)

| Parameter | Type   | Description                     |
| --------- | ------ | ------------------------------- |
| uid       | String | PhotoUID as returned by the API |


# Example
Request: `/api/v1/photos/pqx6gl7v6cl2xt4q`
- `X-Session-Id` header

### Response
<details>
  <summary>Headers</summary>

  <br/>

  | Name              | Value                           |
  | ----------------- | ------------------------------- |
  | Content-Type      | application/json; charset=utf-8 |
  | Date              | Mon, 02 Aug 2021 13:22:58 GMT   |
  | Transfer-Encoding | chunked                         |
</details>  

<details>
  <summary>JSON</summary>

  <br/>

  ```json
  {
    "ID": 105,
    "TakenAt": "2021-02-20T01:29:16Z",
    "TakenAtLocal": "2021-02-20T01:29:16Z",
    "TakenSrc": "",
    "UID": "pqx6gl7v6cl2xt4q",
    "Type": "video",
    "TypeSrc": "",
    "Title": "Not a Cat",
    "TitleSrc": "",
    "Description": "",
    "DescriptionSrc": "",
    "Path": "videos",
    "Name": "20210220-012916-Not-A-Cat-2021",
    "OriginalName": "",
    "Stack": 0,
    "Favorite": false,
    "Private": false,
    "Scan": false,
    "Panorama": false,
    "TimeZone": "UTC",
    "PlaceID": "zz",
    "PlaceSrc": "",
    "CellID": "zz",
    "CellAccuracy": 0,
    "Altitude": 0,
    "Lat": 0,
    "Lng": 0,
    "Country": "zz",
    "Year": 2021,
    "Month": 2,
    "Day": 20,
    "Iso": 0,
    "Exposure": "",
    "FNumber": 0,
    "FocalLength": 0,
    "Quality": 3,
    "Resolution": 0,
    "Color": 0,
    "CameraID": 1,
    "CameraSerial": "",
    "CameraSrc": "",
    "LensID": 1,
    "Details": {
      "PhotoID": 105,
      "Keywords": "black, cat, videos",
      "KeywordsSrc": "",
      "Notes": "",
      "NotesSrc": "",
      "Subject": "",
      "SubjectSrc": "",
      "Artist": "",
      "ArtistSrc": "",
      "Copyright": "",
      "CopyrightSrc": "",
      "License": "",
      "LicenseSrc": "",
      "CreatedAt": "2021-08-01T20:22:19Z",
      "UpdatedAt": "2021-08-01T20:22:20Z"
    },
    "Camera": {
      "ID": 1,
      "Slug": "zz",
      "Name": "Unknown",
      "Make": "",
      "Model": "Unknown"
    },
    "Lens": {
      "ID": 1,
      "Slug": "zz",
      "Name": "Unknown",
      "Make": "",
      "Model": "Unknown",
      "Type": ""
    },
    "Cell": {
      "ID": "zz",
      "Name": "",
      "Category": "",
      "Place": {
        "PlaceID": "zz",
        "Label": "Unknown",
        "City": "Unknown",
        "State": "Unknown",
        "Country": "zz",
        "Keywords": "",
        "Favorite": false,
        "PhotoCount": 17,
        "CreatedAt": "2021-08-01T20:16:47Z",
        "UpdatedAt": "2021-08-01T20:16:47Z"
      },
      "CreatedAt": "2021-08-01T20:16:47Z",
      "UpdatedAt": "2021-08-01T20:16:47Z"
    },
    "Place": {
      "PlaceID": "zz",
      "Label": "Unknown",
      "City": "Unknown",
      "State": "Unknown",
      "Country": "zz",
      "Keywords": "",
      "Favorite": false,
      "PhotoCount": 17,
      "CreatedAt": "2021-08-01T20:16:47Z",
      "UpdatedAt": "2021-08-01T20:16:47Z"
    },
    "Files": [
      {
        "PhotoUID": "pqx6gl7v6cl2xt4q",
        "UID": "fqx6gl831oq12wil",
        "Name": "videos/20210220-012916-Not-A-Cat-2021.mp4.jpg",
        "Root": "sidecar",
        "OriginalName": "",
        "Hash": "cd78c8df6e40f522e71f160d063a947e7136292e",
        "Size": 22383,
        "Codec": "",
        "Type": "jpg",
        "Mime": "image/jpeg",
        "Primary": true,
        "Sidecar": false,
        "Missing": false,
        "Portrait": false,
        "Video": false,
        "Duration": 0,
        "Width": 480,
        "Height": 480,
        "Orientation": 1,
        "AspectRatio": 1,
        "MainColor": "black",
        "Colors": "001106451",
        "Luminance": "01281BEDA",
        "Diff": 687,
        "Chroma": 6,
        "Error": "",
        "ModTime": 1627849340,
        "CreatedAt": "2021-08-01T20:22:20Z",
        "CreatedIn": 295694700,
        "UpdatedAt": "2021-08-01T20:22:20Z",
        "UpdatedIn": 0
      },
      {
        "PhotoUID": "pqx6gl7v6cl2xt4q",
        "UID": "fqx6gl7j84d6qiyi",
        "Name": "videos/20210220-012916-Not-A-Cat-2021.mp4",
        "Root": "/",
        "OriginalName": "",
        "Hash": "51843134d75f4cbde534270cdd5954067f887ee6",
        "Size": 390094,
        "Codec": "avc1",
        "Type": "mp4",
        "Mime": "video/mp4",
        "Primary": false,
        "Sidecar": false,
        "Missing": false,
        "Portrait": false,
        "Video": true,
        "Duration": 5000000000,
        "Width": 480,
        "Height": 480,
        "Orientation": 1,
        "AspectRatio": 1,
        "MainColor": "black",
        "Colors": "001106451",
        "Luminance": "01281BEDA",
        "Diff": 687,
        "Chroma": 6,
        "Error": "",
        "ModTime": 1613784556,
        "CreatedAt": "2021-08-01T20:22:19Z",
        "CreatedIn": 38664500,
        "UpdatedAt": "2021-08-01T20:22:20Z",
        "UpdatedIn": 0
      }
    ],
    "Labels": [
      {
        "PhotoID": 105,
        "LabelID": 18,
        "LabelSrc": "image",
        "Uncertainty": 57,
        "Photo": null,
        "Label": {
          "ID": 18,
          "UID": "lqx6gf82dp687lar",
          "Slug": "cat",
          "CustomSlug": "cat",
          "Name": "Cat",
          "Priority": 5,
          "Favorite": false,
          "Description": "",
          "Notes": "",
          "PhotoCount": 6,
          "CreatedAt": "2021-08-01T20:18:44Z",
          "UpdatedAt": "2021-08-01T20:46:49Z"
        }
      }
    ],
    "CreatedAt": "2021-08-01T20:22:19Z",
    "UpdatedAt": "2021-08-01T20:22:20Z",
    "EditedAt": null,
    "CheckedAt": "2021-08-01T20:31:50Z",
    "DeletedAt": null
  }
  ```
</details>  