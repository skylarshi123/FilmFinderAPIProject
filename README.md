# Movie Recommendation App

This repository contains a JavaScript program that interacts with an external API to provide movie recommendations based on selected genres.

## Overview

The purpose of this application is to allow users to discover random movie recommendations within specific genres. The program leverages APIs from The Movie Database (TMDb) to fetch movie data, including genres and movie information.

## Prerequisites

Before using the application, ensure that you have the following:

- Node.js installed on your machine
- API key from The Movie Database (TMDb)

## Implementation

The implementation of this application involves the following steps:

1. **Fetch Genres:** The `getGenres` function fetches a list of movie genres using the `/genre/movie/list` endpoint from TMDb API. The response is parsed to extract the list of genres.

2. **Fetch Movies:** The `getMovies` function fetches a list of movies based on a selected genre. It uses the `getSelectedGenre` function to determine the chosen genre and constructs the request URL using the `/discover/movie` endpoint with appropriate query parameters.

3. **Display Random Movie:** The `showRandomMovie` function coordinates the process of fetching a list of movies and then displaying information about a randomly selected movie. It uses the `getMovies` function to fetch movies and the `getMovieInfo` function to retrieve detailed information about the selected random movie.

## Usage

To use this application:

1. Clone the repository to your local machine.
2. Obtain an API key from TMDb and replace the `tmdbKey` variable in the code with your API key.
3. Open the HTML file in a web browser.

## Credits

The initial code for interacting with TMDb API and fetching data was provided as part of a pre-written codebase. The focus of this project was on integrating the code and creating the logic to fetch and display movie recommendations.

## Conclusion

This Movie Recommendation App demonstrates how to leverage external APIs to provide users with relevant and engaging content. Feel free to explore, modify, and build upon this project to enhance its features and functionality.
