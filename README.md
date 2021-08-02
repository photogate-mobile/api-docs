Description of main PhotoPrism API endpoints.

# Authorization
Every API request requires `X-Session-Id` authorization header (see "session" endpoint).

- [POST /api/v1/session](auth/create-session.md) // Authorization

# Albums
- [GET /api/v1/albums](albums/get-albums.md) // The list of albums

# Config
- [GET /api/v1/config](config/get-config.md) // PhotoPrism configuration

# Photos
- [GET /api/v1/photos](photos/get-photos.md) // The list of photos
- [GET /api/v1/photos/:uid](photos/get-photo.md) // Full information about photo