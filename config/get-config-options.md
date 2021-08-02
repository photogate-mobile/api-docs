# GET /api/v1/config/options
Retruns PhotoPrism configuration options.

Useful links:
- [API handler implementation](https://github.com/photoprism/photoprism/blob/5076af297963/internal/api/config.go#L40)

# Example
Request: `/api/v1/config/options`
- `X-Session-Id` header

### Response
<details>
  <summary>Headers</summary>

  <br/>

  | Name           | Value                           |
  | -------------- | ------------------------------- |
  | Content-Type   | application/json; charset=utf-8 |
  | Date           | Mon, 02 Aug 2021 15:13:12 GMT   |
  | Content-Length | 749                             |
</details>  

<details>
  <summary>JSON</summary>

  <br/>

  ```json
  {
    "Debug": false,
    "ReadOnly": false,
    "Experimental": false,
    "OriginalsLimit": 1000,
    "Workers": 0,
    "WakeupInterval": 900,
    "AutoIndex": 300,
    "AutoImport": 300,
    "DisableBackups": false,
    "DisableWebDAV": false,
    "DisablePlaces": false,
    "DisableExifTool": false,
    "DisableTensorFlow": false,
    "DisableDarktable": false,
    "DisableRawtherapee": false,
    "DisableSips": false,
    "DisableHeifConvert": false,
    "DisableFFmpeg": false,
    "DetectNSFW": false,
    "SiteUrl": "http://localhost:2342/",
    "SitePreview": "",
    "SiteTitle": "PhotoPrism",
    "SiteCaption": "Browse Your Life",
    "SiteDescription": "",
    "SiteAuthor": "",
    "RawPresets": false,
    "FFmpegEncoder": "libx264",
    "FFmpegBitrate": 50,
    "FFmpegBuffers": 32,
    "ThumbFilter": "lanczos",
    "ThumbUncached": false,
    "ThumbSize": 2048,
    "ThumbSizeUncached": 7680,
    "JpegSize": 7680,
    "JpegQuality": 92
  }
  ```
</details>  