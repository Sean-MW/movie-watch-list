# Movie Watch List
A simple Java Swing desktop app that tracks and rates movies a user has watched that I built for CPSC 210 at the 
University of British Columbia.

## Demo
To add a movie click the add movie button at the bottom of the frame.

![Demo 1](data/images/demo1.png)
A new window will pop up. Search for a movie using the search bar and Search Movie button. Select the movie and click the Add Selected button to add it to the watch list.

![Demo 2](data/images/demo2.png)
The movie is now on the watch list. To rate it, select the movie and click the Edit Movie button.

![Demo 3](data/images/demo3.png)
A new window containing movie details will pop up. Select a rating from the dropdown menu and click the Change Rating
button.

![Demo 4](data/images/demo4.png)
The movie will now display the chosen rating on the watch list.

![Demo 5](data/images/demo5.png)
Use the Load Watch List and Save Watch List buttons to save and load the watch list to/from a JSON file.

## Logs
The application prints out all changes made to the watch list to the console when it exits.

![UML Design Diagram](data/images/logs.png)

## Project Structure
The application is structured to have three frames: MainFrame, EditFrame, SearchFrame.
Each frame consists of a few panels, which each have their own separate purposes.
The application is based around finding movies, adding and removing them from lists, and making changes to them.
All of this is done within the WatchList, MovieSearchList, MovieList, and Movie classes.

![UML Design Diagram](data/images/uml-design-diagram.png)

## Data
All movie data and icons are from
[this](https://www.kaggle.com/harshitshankhdhar/imdb-dataset-of-top-1000-movies-and-tv-shows?select=imdb_top_1000.csv)
Kaggle dataset.

## Future Plans
- Expand number of available movies (currently 1000)
  - Create database
  - Write python script to scrape IMDb and update database
- Recommendation system using clustering algorithm (e.g. KNN)
