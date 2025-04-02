# Python-Project

This Python-based Movie Information Retrieval App provides users with an interactive way to search for movies and gather detailed information about them. By using the Open Movie Database (OMDB) API, this project retrieves in-depth data about movies, including release year, plot summary, runtime, genres, directors, actors, language options, awards, and more. The main goal of this application is to offer users an easy-to-use platform to gather essential details about their favorite movies and assist them with conducting research on films in a user-friendly and efficient way.

# Key Features and Functionality:

## User Interaction & Customization:

The program prompts users to input their name, followed by a personalized welcome message.

Users can choose from a menu of options, such as viewing previously searched movies, searching for new movie titles, or quitting the app.

The program is designed to be user-friendly, offering a simple and engaging interface with easy-to-understand options.

## Search and Display Movie Information:

Users can search for a specific movie title, and the program fetches detailed information from the OMDB API. The data includes:

- The movie's release year
- Plot summary
- Runtime
- Genre
- Directors, writers, and actors
- Language options
- Awards won (if any)

The app then displays this information clearly, allowing users to explore the movie in detail.

## Persistent Movie History:

The app saves previously searched movie titles to a text file, allowing users to view and select past searches.

Users can decide whether to search for a new movie or re-examine a movie they’ve previously searched.

## Error Handling & Data Validation:

In the case of invalid movie titles, the app gracefully handles errors by using a try-except mechanism, ensuring the program doesn't crash. Instead, users are prompted to re-enter a valid title.

This feature enhances the app's reliability and ensures a smooth user experience.

## Creative User Experience:

Instructions to users are creatively printed letter-by-letter, with a short time interval between each letter, using the time.sleep function. This is done to capture the user’s attention and make the experience more interactive and engaging.

The use of the flush function ensures that the instructions are displayed without delays or buffering.

## File Management:

The program uses the os module to manage files, ensuring that previously searched movies are stored and displayed neatly. The os.listdir() function lists saved files, and unnecessary files (not related to movie searches) are removed using the .remove() method.

The with open function is used to save and manage the movie search history, ensuring that the file is closed automatically after data is written, preventing data loss or errors.

## API Integration:

The Open Movie Database (OMDB) API is used as the data source for retrieving movie information. The program sends a request to the OMDB API, receives the data in JSON format, and processes it accordingly.

The app utilizes authentication through an API key to securely access the OMDB API and fetch real-time movie information.

## Flexible Options for the User:

The app provides a simple menu system where the user can choose between:
- Viewing previously searched movie titles.
- Searching for a new movie.
- Exiting the program.

Each choice is handled by the program in a way that ensures the user can continue interacting without confusion, and the system is robust enough to avoid crashes when invalid inputs are entered.

## Data Collection and API Usage:
The project makes use of the Open Movie Database (OMDB) API, a free and public API that provides detailed information about movies, TV shows, and series. The OMDB API plays a crucial role in this project by providing access to real-time movie data, which the app uses to respond to user queries. The interaction with the API is facilitated through the requests.get() function, which sends HTTP requests to fetch movie data, and the data is returned in JSON format, which is parsed and displayed to the user.

The OMDB API makes it possible to get a wide range of information about movies, such as release dates, cast members, genres, and accolades. This enriches the app's ability to provide comprehensive movie details, making it an ideal tool for movie enthusiasts, researchers, or anyone seeking more knowledge about films.
