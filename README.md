# cult-films-bs4
This Python code fetches data from "https://web.archive.org/web/20200518073855/https://www.empireonline.com/movies/features/best-movies-2/".

The code retrieves data from a list on the Empire Online website that contains the best movies. Firstly, the requests.get() method is used to fetch the source code of the web page. Then, the BeautifulSoup library is used to parse and convert this source code into HTML.

The code finds all the movie titles (all_movies) using BeautifulSoup's find_all() method and extracts the text of each movie using the getText() method. The movie titles are stored in the movie_titles list.

The movies list is created by reversing the order of the movie_titles list. This will give us the movies in reverse order.

Finally, the movie titles are written to a file named "movies.txt" using the open() function and a for loop. Each movie title is written on a new line in the file.

Make sure you have installed the BeautifulSoup and requests libraries for the code to run properly.
