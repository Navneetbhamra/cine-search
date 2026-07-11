Cine Search

Cine Search is a dynamic movie discovery application built with React and Vite. It allows users to search for movies using The Movie Database (TMDB) API and view a list of trending titles. The "Trending Movies" feature is powered by Appwrite, which tracks search query popularity to provide relevant results.

Features

Movie Search: Instantly search for movies from the extensive TMDB library.
Trending Section: A dynamic list of trending movies is generated based on the most frequent search terms, tracked via Appwrite.
Detailed Movie Cards: Displays key movie information such as the poster, title, average rating, original language, and release year.
Responsive Design: The interface is fully responsive, providing a great experience on any device.

Tech Stack

Frontend: React, Vite
Styling: Tailwind CSS
Backend as a Service (BaaS): Appwrite
Data Source: The Movie Database (TMDB) API

Getting Started

To get a local copy up and running, follow these steps.

Prerequisites

You will need to have Node.js and npm installed on your machine. You will also need API keys and project credentials from the following services:
[The Movie Database (TMDB)](https://www.themoviedb.org/signup)
[Appwrite cloud](https://cloud.appwrite.io/console/)

Installation & Setup

Clone the repository:

`git clone https://github.com/navneetbhamra/cine-search.git`

Navigate to the project directory:

`cd cine-search`

Install NPM packages:

`npm install`

Create an environment file: Create a `.env` file in the root of the project and add the following environment variables:

VITE_TMDB_API_KEY=YOUR_TMDB_API_KEY
VITE_APPWRITE_PROJECT_ID=YOUR_APPWRITE_PROJECT_ID
VITE_APPWRITE_DATABASE_ID=YOUR_APPWRITE_DATABASE_ID
VITE_APPWRITE_COLLECTION_ID=YOUR_APPWRITE_COLLECTION_ID

In your Appwrite project, create a database and a collection. The collection should have attributes for searchTerm (string), count (integer), movie_id (integer), and poster_url (string) to track search analytics.

Running the Application

Start the development server

`npm run dev`

Open your browser and navigate to the local URL provided by Vite (usually http://localhost:5173).
