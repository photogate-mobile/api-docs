# GET /api/v1/t/:hash/:token/:type
Returns thumbnail for given media file (photo or video). 

Useful links:
- [API handler implementation](https://github.com/photoprism/photoprism/blob/fe8599961dae/internal/api/photo_thumb.go#L23)
- [Thumbnails types](https://github.com/photoprism/photoprism/blob/fe8599961daef94f3c134e36b9e741478838f72e/internal/thumb/types.go)

| Parameter | Type   | Description                                          |
| --------- | ------ | ---------------------------------------------------- |
| hash      | String | SHA1 file hash                                       |
| token     | String | Preview token. See [config](../config/get-config.md) |
| type      | String | Thumbnail type. See table below                      |


| Type                       | Use                      | Source   | Dimensions (WxH) | Public |
| -------------------------- | ------------------------ | -------- | ---------------- | ------ |
| tile_50                    | Lists                    | tile_500 | 50x50            | false  |
| tile_100                   | Maps                     | tile_500 | 100x100          | false  |
| tile_224                   | TensorFlow, Mosaic       | tile_500 | 224x224          | false  |
| tile_500                   | Tiles                    | -        | 500x500          | false  |
| colors                     | Color Detection          | fit_720  | 3x3              | false  |
| left_224                   | TensorFlow               | fit_720  | 224x224          | false  |
| right_224                  | TensorFlow               | fit_720  | 224x224          | false  |
| fit_720                    | Mobile, TV               | -        | 720x720          | true   |
| fit_1280                   | Mobile, HD Ready TV      | fit_2048 | 1280x1024        | true   |
| fit_1920                   | Mobile, Full HD TV       | fit_2048 | 1920x1200        | true   |
| fit_2048                   | Tablets, Cinema 2K       | -        | 2048x2048        | true   |
| fit_2560                   | Quad HD, Retina Display  | -        | 2560x1600        | true   |
| fit_3840 <br> (Deprecated) | Ultra HD                 | -        | 3840x2400        | false  |
| fit_4096                   | Ultra HD, Retina 4K      | -        | 4096x4096        | true   |
| fit_7680                   | 8K Ultra HD 2, Retina 6K | -        | 7680x4320        | true   |



# Example
Request: `/api/v1/t/51843134d75f4cbde534270cdd5954067f887ee6/2e78f2ac/tile_224`
- `X-Session-Id` header

### Response
<details>
  <summary>Headers</summary>

  <br>

  | Name           | Value                                             |
  | -------------- | ------------------------------------------------- |
  | Accept-Ranges  | bytes                                             |
  | Cache-Control  | private, max-age=7776000, no-transform, immutable |
  | Content-Length | 17382                                             |
  | Content-Type   | image/jpeg                                        |
  | Last-Modified  | Sun, 01 Aug 2021 20:22:20 GMT                     |
  | Date           | Fri, 06 Aug 2021 01:21:56 GMT                     |
</details>  

<details>
  <summary>Thumbnail</summary>

  <br>

  ![Thumbnail response](thumb-example.png)
</details>  