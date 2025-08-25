# Frostal.us [![.github/workflows/deploy.yml](https://github.com/Frostal-us/Frostal/actions/workflows/deploy.yml/badge.svg)](https://github.com/Frostal-us/Frostal/actions/workflows/deploy.yml)

Live, social photo sharing.

- Website: https://Frostal.us
- Topics: live • media • share • social

## Project: Frostal

Dev quickstart (Bun v1.2.14):
```bash
bun install
bun run index.ts
```

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
