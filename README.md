<div align="center">
  <img src="public/hero.png" alt="Hero Image" width="300" />
</div>

# Movie Streamer

A high-performance, responsive web application for discovering movies and tracking real-time search trends. Built with **React 19**, **Tailwind CSS v4**, and **Appwrite**, this project integrates the **TMDB API** to deliver seamless browsing with optimized search capabilities.


## 🚀 Key Features

- **Dynamic TMDB Integration**: Fetches and displays real-time movie data, ratings, and artwork in clean, interactive grid cards.

- **Optimized Search with Debouncing**: Features a custom search engine that minimizes API overhead and enhances UX by delaying API calls until the user stops typing.

- **Trending Movies Analytics**: Leverages Appwrite as a backend database to track user search terms, aggregate metrics, and dynamically display the platform's top trending movies.

- **Modern UI/UX**: Fully responsive, modern dark-themed interface built using the latest Tailwind CSS v4 design tokens.

## 🛠️ Tech Stack & Architecture 

### Frontend

- **React 19**: Utilizing modern hooks (useState, useEffect) and concurrent rendering patterns for smooth state transitions.

- **Vite 8.0**: Next-generation frontend tooling providing lightning-fast Hot Module Replacement (HMR) and optimized production builds.

- **Tailwind CSS v4.3**: Leverages the latest CSS-first configuration and high-performance utility classes.

### Backend-as-a-Service (BaaS)
- **Appwrite v1.9**: Handles database storage for tracking and incrementing search term frequencies to power the "Trending" algorithm.

### API
- **TMDB API v3**: Industry-standard movie database endpoint utilized for rich media data retrieval.

## 📦 Installation & Setup

### Prerequisites
* **Node.js** `v22.22.3`
* **npm** `11.16.0`

### 1. Clone the Repository
First, clone the repository to your local machine using your terminal:

```bash
git clone https://github.com/AmaraFinbarrs/movie-streamer.git

cd movie-streamer
```

### 2. Install Dependencies
Install all the required frontend and backend-as-a-service packages:

```bash
 npm install
```
 
 
### 3. Configure Environment Variables
Create a file named `.env.local` in the root directory of your project and populate it with your TMDB and Appwrite credentials:

```
VITE_TMDB_API_KEY = eyJhbGciOiJIUzI1NiJ9.eyJhdWQiOiI4MjE3ZWI2OWRkZjFkNzcwOWNhNzNjMDYyMDM2ZGRjNiIsIm5iZiI6MTc4MTkyMTMxMi42NTY5OTk4LCJzdWIiOiI2YTM1ZjYyMDlkMWQ0MjJiMTc0ZDg4YzkiLCJzY29wZXMiOlsiYXBpX3JlYWQiXSwidmVyc2lvbiI6MX0.u1ZdIwlo6hM_S9Zk21aImuCalPaiih3DOHsLziLpz1c
VITE_APPWRITE_PROJECT_ID = "6a37303b003df015c073"
VITE_APPWRITE_PROJECT_NAME = "Movie Streamer"
VITE_APPWRITE_ENDPOINT = "https://fra.cloud.appwrite.io/v1"
VITE_APPWRITE_DATABASE_ID = "6a3733060021bc503bf6"
VITE_APPWRITE_COLLECTION_ID = "metrics"
```

### 4. Start the Development Server
Run the following command to boot up the application locally using Vite:

```bash
npm run dev
```

Once started, open your browser and navigate to http://localhost:5173 (or the port specified in your terminal output) to view the application.