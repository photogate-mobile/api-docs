Description of main PhotoPrism API endpoints.

# Authorization
Every API request requires `X-Session-Id` authorization header (see "session" endpoint).

- [POST /api/v1/session](auth/create-session.md) // Authorization

# Albums
- [GET /api/v1/albums](albums/get-albums.md) // The list of albums

# Config
- [GET /api/v1/config](config/get-config.md) // The list of cameras, lenses, countries, etc
- [GET /api/v1/config/options](config/get-config-options.md) // PhotoPrism configuration options

# Photos
- [GET /api/v1/photos](photos/get-photos.md) // The list of photos
- [GET /api/v1/photos/:uid](photos/get-photo.md) // Full information about photo
- [GET /api/v1/photos/:uid/dl](photos/get-photo-download.md) // Download full-size photo
- [GET /api/v1/t/:hash/:token/:type](photos/get-thumb.md) // Download thumbnail for given media file

# Videos 
- [GET /api/v1/videos/:hash/:token/:type](videos/get-video.md) // Download/Stream video file 