# Frostal.us ![GitHub](https://img.shields.io/badge/GitHub-xeoxaz-blue?logo=github&logoColor=white)

Live, social photo sharing.

- Website: https://Frostal.us
- Topics: live • media • share • social

## Project: Frostal

### Photos
- Public files: public/uploads/<username>/photos
- Metadata: MongoDB collection photos
- No meta.json used

API endpoints:
- GET /api/users/:username/photos — list public photos (respects private profiles)
- GET /api/users/me/photos — list your photos
- POST /api/users/me/photos — upload a photo
- POST /api/users/me/photos/title — set/clear a photo title
- DELETE /api/users/me/photos — delete a photo by name
