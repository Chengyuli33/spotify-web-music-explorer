# 🎨 Client - React Frontend

This directory contains the React frontend for the Web Database Application.

## 🧭 Features

- **Homepage with song of the day**, top songs, and albums
- **Advanced filtering** for songs by title, energy, danceability, valence, etc.
- **Bar and radar charts** for visualizing audio features
- **Lazy loading tables** with pagination
- **Multi-page routing** via React Router

## 🗂️ Key Files
| Path | Description |
|------|-------------|
| [`src/pages/HomePage.js`](./src/pages/HomePage.js) | Landing page with song of the day and top content (songs & albums). |
| [`src/pages/SongsPage.js`](./src/pages/SongsPage.js) | Song search page with multi-criteria filters and results in a sortable table. |
| [`src/pages/AlbumsPage.js`](./src/pages/AlbumsPage.js) | Grid layout of all albums using flexbox-based responsive formatting. |
| [`src/pages/AlbumInfoPage.js`](./src/pages/AlbumInfoPage.js) | Album detail page with cover image, metadata, and track list. |
| [`src/components/SongCard.js`](./src/components/SongCard.js) | Modal component to display song details and audio visualizations (bar & radar chart). |
| [`src/components/LazyTable.js`](./src/components/LazyTable.js) | Reusable paginated table component that fetches data lazily from the backend. |
| [`src/components/NavBar.js`](./src/components/NavBar.js) | App-wide navigation bar built using MUI’s `AppBar` and `Typography`. |
| [`src/helpers/formatter.js`](./src/helpers/formatter.js) | Helper functions to format duration and release dates. |
| [`src/config.json`](./src/config.json) | Stores backend server connection info (host and port). |
| [`App.js`](./src/App.js) | Root component that defines theme and structure for the frontend app. |
| [`index.js`](./src/index.js) | React entry point with route configuration and DOM rendering. |