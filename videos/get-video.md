# GET /api/v1/videos/:hash/:token/:type 
Returns (streames) given video file.

Useful links:
- [API handler implementation](https://github.com/photoprism/photoprism/blob/fe8599961dae/internal/api/video.go#L20)
- [Video types](https://github.com/photoprism/photoprism/blob/fe8599961daef94f3c134e36b9e741478838f72e/internal/video/video.go#L64)

| Parameter | Type   | Description                                           |
| --------- | ------ | ----------------------------------------------------- |
| hash      | String | SHA1 file hash                                        |
| token     | String | Download token. See [config](../config/get-config.md) |
| type      | String | Video type. See table below                           |

| Type           | Description |
| -------------- | ----------- |
| (not provided) | TypeAvc     |
| mp4            | TypeMp4     |
| avc            | TypeAvc     |


# Example
Request: `/api/v1/videos/51843134d75f4cbde534270cdd5954067f887ee6/3lk3gz25/mp4`
- `X-Session-Id` header

### Response
<details>
  <summary>Headers</summary>

  <br>

  | Name           | Value                         |
  | -------------- | ----------------------------- |
  | Accept-Ranges  | bytes                         |
  | Content-Length | 390094                        |
  | Content-Type   | video/mp4; codecs="avc1       |
  | Last-Modified  | Sat, 20 Feb 2021 01:29:16 GMT |
  | Date           | Fri, 06 Aug 2021 01:45:16 GMT |
</details>  

<details>
  <summary>Data</summary>

  <br>

  `Video stream`
</details>  