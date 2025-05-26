
## 📡 Backend API Endpoints:

All endpoints are implemented in [`routes.js`](./server/routes.js) and served via Express [`server.js`](./server/server.js).


| Method | Endpoint                  | Description                            |
|--------|---------------------------|----------------------------------------|
| GET    | `/song/:song_id`          | Get full metadata for a song           |
| GET    | `/album/:album_id`        | Get full metadata for an album         |
| GET    | `/albums`                 | List all albums (sorted by release date) |
| GET    | `/album_songs/:album_id`  | List songs in an album (ordered by track) |
| GET    | `/top_songs?page=N`       | Top songs by play count (paginated)    |
| GET    | `/top_albums?page=N`      | Top albums by total plays (paginated)  |
| GET    | `/search_songs?...`       | Filter songs by duration, energy, etc. |
| GET    | `/random?explicit=true`   | Get a random song |
| GET    | `/author/:type`           | Returns app author's name |



## 🗂️ Key Files and Folders
| Path | Description |
|------|-------------|
| [`server.js`](./server.js) | Entry point for the backend server. Registers all API routes and starts the Express app. |
| [`routes.js`](./routes.js) | Main route handler file. Contains all SQL-based API endpoint logic (e.g. `/top_songs`, `/search_songs`). |
| [`config.json`](./config.json) | Stores PostgreSQL RDS credentials and backend server configuration. |
| [`package.json`](./package.json) | Lists backend dependencies and project metadata. |
