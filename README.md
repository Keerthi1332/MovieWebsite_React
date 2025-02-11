# Movies Website

This is a movies website built using ReactJS that fetches movie information from an API and displays a list of trending movies. The app stores the count of the trending movies and displays the most popular ones. The website is hosted on Netlify for easy deployment and sharing.

## Features

- Fetch movie data from an external API.
- Display trending movies based on popularity.
- Store and manage movie count for trending movies using Appwrite.
- Hosted on Netlify for seamless access.

## Tech Stack

- **Frontend**: ReactJS (Vite), tailwind CSS
- **State Management**: React State (useState, useEffect)
- **Database**: Appwrite
- **API**: The Movie Database (TMDb) API (or any other movie API of your choice)
- **Hosting**: Netlify

## Getting Started

To get the project up and running on your local machine, follow these steps:

**1.Clone the Repository**: 
  First, clone the repository to your local machine using the following command:
  
   git clone https://github.com/your-username/movies-website.git

**2. Install Dependencies:**
  Navigate to the project directory and install the necessary dependencies using npm or yarn:
  
    cd movies-website
    
    npm install

**3. Set Up Appwrite Database:**
  Install and set up Appwrite by following the instructions in the Appwrite documentation. After setting up the database, make sure you configure the necessary collections and      permissions.
  
  Create a Movies collection with the required attributes (e.g., title, release date, poster, and count).
  
  Obtain the Appwrite Project ID and API endpoint.
  
  Configure Appwrite in the Project:
  
  Add the Appwrite API endpoint and Project ID to the .env file:
  
  REACT_APP_APPWRITE_API_ENDPOINT=your_appwrite_api_endpoint
  
  REACT_APP_APPWRITE_PROJECT_ID=your_appwrite_project_id

**4. Run the App Locally:**

  Once dependencies are installed and the API key is set up, start the app using the following command:
  
  npm start (or) npm run dev
  
  This will start the React development server and open the app in your browser at http://localhost:3000.

**App Structure:**

  /src: Contains all the source files for the app.
  
  /components: Contains various components such as:
  
    MovieCard: Displays individual movie details like title, poster, and release date.
    
    Spinner: Shows a loading spinner while data is being fetched.
    
    Search: Handles the search functionality for searching movies.
    
  /App.js: Main app file where multiple components are integrated.
  
  /index.js: Entry point to the application.

**Components:**

  MovieCard: Displays individual movie details such as title, poster, and release date.
  
  Spinner: A loading spinner displayed when fetching movie data from the API.
  
  Search: A search bar to allow users to search for movies.
  
  App: Main component that integrates all the features of the app and renders other components.

**Hosting on Netlify:**
  To host the app on Netlify, follow these steps:
  
  Push the code to a Git repository (GitHub, GitLab, Bitbucket, etc.).
  
  Go to Netlify.
  
  Click on New site from Git.
  
  Select the repository and configure the build settings:
  
  Build Command: npm run build
  
  Publish Directory: build
  
  Deploy your site.
  
  Once deployed, the website will be live on Netlify, and will get a public URL to share!

**URL** - https://moviewebsitereact.netlify.app


