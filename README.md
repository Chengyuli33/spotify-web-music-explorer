# 🎧 Spotify WebDB Application

A full-stack music data exploration platform developed in React + Node.js, integrated with a PostgreSQL RDS backend. This project demonstrates dynamic querying, data visualization, and backend API design. Designed as part of CIS 5500: Database and Information Systems coursework.

## 🔧 Tech Stack
- Database: PostgreSQL on AWS RDS
- Frontend: React.js, MUI (Material UI), Recharts
- Backend: Node.js + Express
- Visualization: Recharts (RadarChart, BarChart)
- Dev Tools: VS Code, Git, Chrome DevTools, DataGrip, npm

## ✨ Features
- Powerful search filters: by title, duration, plays, energy, valence, danceability, etc.
- Top albums/songs ranking with pagination
- Song detail page with dynamic bar chart and radar chart 
- Pagination support and lazy-loaded tables for performance
- Fully documented REST API with route handlers

![Home](screenshots/homepage.png)

![Radar Chart](screenshots/radarchart.png)

![ER Diagram](screenshots/ER_diagram.png)


## 📂 Project Structure

`/server`

`/client`

`/data`

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



## 📊 Database
[`Dataset Description`](data./README.md) 👉 Detailed expliation of the metadata feature and data loading in Datagrip.




## 🚀 Getting Started

### 1. Clone and install server dependencies
This will download and save the required dependencies into the `node_modules` folder within the `/client` and `/server` directories.

```bash
cd server
npm install
```

![server dependencies](screenshots/server_dependencies.png)

Then start the server
```bash
npm start
```



### 2. In another terminal, install client dependencies

```bash
cd ../client
npm install
```

![client dependencies](screenshots/client_dependencies.png)


Start React frontend
```bash
npm start
```

### 3. Access the app in your browser

The app will run at:
- Frontend: http://localhost:3000
- Backend: http://localhost:8080
