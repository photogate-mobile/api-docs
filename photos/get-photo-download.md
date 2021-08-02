# GET /api/v1/photos/:uid/dl
Returns full-size photo file.

Useful links:
- [API handler implementation](https://github.com/photoprism/photoprism/blob/5076af297963/internal/api/photo.go#L126)

| Parameter | Type   | Description    |
| --------- | ------ | -------------- |
| t         | String | Download token |


# Example
Request: `/api/v1/photos/pqx6gl7v6cl2xt4q/dl?t=3f2omhvj`
- `X-Session-Id` header

### Response
<details>
  <summary>Headers</summary>

  <br/>

  | Name                | Value                                                         |
  | ------------------- | ------------------------------------------------------------- |
  | Accept-Ranges       | bytes                                                         |
  | Content-Disposition | attachment; filename="20210220-012916-Not-A-Cat-2021.mp4.jpg" |
  | Content-Length      | 22383                                                         |
  | Content-Type        | image/jpeg                                                    |
  | Last-Modified       | Sun, 01 Aug 2021 20:22:20 GMT                                 |
  | Date                | Mon, 02 Aug 2021 23:38:31 GMT                                 |
</details>  

<details>
  <summary>Photo</summary>

  <br/>

  ![Photo response](example-photo.png)

</details>  