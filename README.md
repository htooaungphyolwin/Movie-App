# Movie Search Application

A modern React application that allows users to search and discover movies using TMDB API, with trending searches powered by Appwrite backend integration.

## Features

- **Movie Search**: Search through thousands of movies with real-time results
- **Trending Movies**: Track and display most searched movies
- **Movie Details**: View detailed information including ratings, release year, and language
- **Responsive Design**: Modern UI that works across all devices

## Tech Stack

- React 18
- Vite
- Tailwind CSS
- Appwrite (Backend as a Service)
- TMDB API

## Prerequisites

- Node.js (v14 or higher)
- npm or yarn
- Appwrite instance
- TMDB API key

## Environment Variables

Create a `.env` file in the root directory with the following variables:

```env
VITE_API_KEY=your_tmdb_api_key
VITE_APPWRITE_ENDPOINT=your_appwrite_endpoint
VITE_APPWRITE_PROJECT_ID=your_appwrite_project_id
VITE_APPWRITE_DATABASE_ID=your_appwrite_database_id
VITE_APPWRITE_COLLECTION_ID=your_appwrite_collection_id
```

## Setup Instructions

1. Clone the repository
2. Install dependencies:

   ```bash
   npm install
   ```

3. Set up environment variables as described above
4. Start the development server:

   ```bash
   npm run dev
   ```

## Project Structure

```
├── src/
│   ├── components/         # React components
│   │   ├── MovieCard.jsx   # Individual movie display
│   │   ├── Search.jsx      # Search input component
│   │   ├── Spinner.jsx     # Loading indicator
│   │   └── TrendingMovies.jsx  # Trending movies section
│   ├── appWrite.js         # Appwrite configuration and functions
│   ├── App.jsx            # Main application component
│   └── main.jsx           # Application entry point
├── public/                # Static assets
└── vite.config.js        # Vite configuration
```

## Components

### MovieCard

Displays individual movie information including:

- Movie poster
- Title
- Rating
- Original language
- Release year

### Search

Provides a search input field with debounced search functionality.

### TrendingMovies

Displays a list of most searched movies tracked through Appwrite.

## API Integration

### TMDB API

- Used for fetching movie data
- Supports movie search and discovery

### Appwrite Integration

- Tracks search trends
- Stores most searched movies
- Manages movie metadata

## Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build
- `npm run lint` - Run ESLint

## Contributing

1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Create a new Pull Request

## License

This project is open source and available under the MIT License.
