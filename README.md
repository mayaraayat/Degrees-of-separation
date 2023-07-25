# Degrees-of-separation
# CS50 AI - Week 0 - Degrees

## Background 

According to the Six Degrees of Kevin Bacon game, anyone in the Hollywood film industry can be connected to Kevin Bacon within six steps, where each step consists of finding a film that two actors both starred in.

In this problem, we’re interested in finding the shortest path between any two actors by choosing a sequence of movies that connects them. For example, the shortest path between Jennifer Lawrence and Tom Hanks is 2: Jennifer Lawrence is connected to Kevin Bacon by both starring in “X-Men: First Class,” and Kevin Bacon is connected to Tom Hanks by both starring in “Apollo 13.”

We can frame this as a search problem: our states are people. Our actions are movies, which take us from one actor to another (it’s true that a movie could take us to multiple different actors, but that’s okay for this problem). Our initial state and goal state are defined by the two people we’re trying to connect. By using breadth-first search, we can find the shortest path from one actor to another.

## The project

This project was created with the help of CS50 AI - Week 0 Program.
This Python script, degrees.py, is a program that helps find the shortest path between two actors or actresses in terms of their movie collaborations, also known as "Six Degrees of Kevin Bacon." The script uses CSV files containing information about people (actors/actresses), movies, and their collaborations to calculate the degrees of separation between two given individuals.

## How to Use

Step 1: Data Loading
Before running the script, make sure to place the required CSV files (people.csv, movies.csv, stars.csv) in the same directory as the script. These CSV files contain information about people, movies, and their collaborations. The data will be loaded into memory when the program starts.

Step 2: Running the Program
To execute the program, open a terminal or command prompt, navigate to the directory containing the degrees.py script and CSV files, and run the following command:
python degrees.py [directory]

If no directory name is provided, the script will default to the "large" directory. The script will prompt you to enter the names of two actors or actresses (source and target) for whom you want to find the degrees of separation.

Step 3: Finding Degrees of Separation
The script will then calculate the shortest path between the two provided names based on their movie collaborations. If a path is found, it will display the number of degrees of separation and the list of movies connecting the two individuals.

Example Usage
python degrees.py
Output:
Loading data...
Data loaded.
Name: Tom Hanks
Name: Meryl Streep
1 degree of separation.
1: Tom Hanks and Meryl Streep starred in The Post

## Functionality and Structure

The script uses a breadth-first search algorithm to find the shortest path between the source and target actors/actresses. It represents each actor/actress and movie as a node in a graph, and their collaborations form edges between nodes.

## Notes

Please ensure that you have Python 3.x installed on your system along with the required CSV files in the same directory as the script. If you encounter any issues or errors, verify that the CSV files are correctly formatted and contain the necessary information.

Feel free to use and modify this script to explore the fascinating world of "Six Degrees of Kevin Bacon" and discover how actors and actresses are connected through their movie collaborations. Enjoy!
