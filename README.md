<h1 align="center">Movie Recommendation System</h1>
<p align="center">
 <a target="_blank" href="/">Link to the App</a>
    ·
 <a target="_blank" href="/">Video Demo</a>
</p>

<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#salient-features">Salient Features</a></li>
        <li><a href="#compatible-platforms">Compatible Platforms</a></li>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#how-to-get-the-API-key?">How to get the API key</a></li>
        <li><a href="#how-to-run-the-project?">How to run the project</a></li>
      </ul>
   </li>
    <li><a href="#architecture">Architecture</li>
    <li><a href="#content-based-filtering">Content based Filtering</li>
    <li><a href="#similarity-score">Similarity Score</li>
    <li><a href="#how-cosine=similarity-works">How Cosine Similarity works?</li>
     
    <li><a href="#navigating-through-the-app">Navigating through the App</a></li>
    <ul>
      <li><a href="#home-page">Home page</a></li>
      <li><a href="#searching-for-a-movie">Searching for a movie</a></li>
      <li><a href="#details-of-the-movie-searched">Details of the movie searched</a></li>
      <li><a href="#movie's-cast">Movie's Cast</a></li>
      <li><a href="#recommended-movies">Recommended Movies</a></li>
      <li><a href="#user-reviews">User Reviews</a></li>
    </ul>
    <li><a href="#sources-of-the-datasets">Sources of the datasets</a></li>
    <li><a href="#resources-used">Resources Used</a></li>
  </ol>
</details>

## About the project
* Movie Recommendation Engine - AMFLIX built during Microsoft Engage 2022 program
* It is a recommendation engine made using Content based Filtering approach

### Salient Features
* Recommends movies based on the likes of the user
* Gives the details of the movie and its cast searched by the user using API
* Analyses the sentiments of the reviews given by user

### Compatible Platforms
Laptops, Desktops and Tablet PCs

### Built With
* ![Python](https://img.shields.io/badge/Python-3.8-blueviolet)
* ![Framework](https://img.shields.io/badge/Framework-Flask-red)
* ![Frontend](https://img.shields.io/badge/Frontend-HTML/CSS/JS-green)
* ![API](https://img.shields.io/badge/API-TMDB-fcba03)

## Getting Started

### How to get the API key?

Create an account in https://www.themoviedb.org/, click on the `API` link from the left hand sidebar in your account settings and fill all the details to apply for API key. If you are asked for the website URL, just give "NA" if you don't have one. You will see the API key in your `API` sidebar once your request is approved.

### How to run the project?

1. Clone or download this repository to your local machine.
2. Install all the libraries mentioned in the [requirements.txt](https://github.com/RishikaKant/AMFLIX/blob/master/requirements.txt) file with the command `pip install -r requirements.txt`
3. Get your API key from https://www.themoviedb.org/. (Refer the above section on how to get the API key)
3. Replace YOUR_API_KEY in **both** the places (line no. 15 and 29) of `static/recommend.js` file and hit save.
4. Open your terminal/command prompt from your project directory and run the file `main.py` by executing the command `python main.py`.
5. Go to your browser and type `http://127.0.0.1:5000/` in the address bar.
6. Hurray! That's it.


## Architecture

![Recommendation App](https://user-images.githubusercontent.com/36665975/168742738-5435cf76-1a42-4d87-94b4-999e5bfc48d3.png)

## Content based Filtering
Content-based recommendation systems uses their knowledge about each product to recommend new ones. Recommendations are based on attributes of the item. Content-based recommender systems work well when descriptive data on the content is provided beforehand. “Similarity” is measured against product attributes.

Suppose I watch a movie in a particular genre, then I will be recommended movies within that specific genre. The movie's attributes, like title, year of release, director and cast, are also helpful in identifying similar movie content

## Similarity Score : 

   How does it decide which item is most similar to the item user likes? Here come the similarity scores.
   
   It is a numerical value ranges between zero to one which helps to determine how much two items are similar to each other on a scale of zero to one. This similarity score is obtained measuring the similarity between the text details of both of the items. So, similarity score is the measure of similarity between given text details of two items. This can be done by cosine-similarity.
   
## How Cosine Similarity works?
  Cosine similarity is a metric used to measure how similar the documents are irrespective of their size. Mathematically, it measures the cosine of the angle between two vectors projected in a multi-dimensional space. The cosine similarity is advantageous because even if the two similar documents are far apart by the Euclidean distance (due to the size of the document), chances are they may still be oriented closer together. The smaller the angle, higher the cosine similarity.
  
  ![image](https://user-images.githubusercontent.com/36665975/70401457-a7530680-1a55-11ea-9158-97d4e8515ca4.png)

  
More about Cosine Similarity : [Understanding the Math behind Cosine Similarity](https://www.machinelearningplus.com/nlp/cosine-similarity/)

<!-- APP TUTORIAL-->
## Navigating Through The App

### Home page
<img src="images/home_page.png" alt="home page" width="700"/>

### Searching for a movie
* The search bar has autocomplete feature.
<img src="images/search.png" alt="search" width="700"/>

### Details of the movie searched
<img src="images/movie_details.png" alt="movie details" width="700"/>

### Movie's Cast
<img src="images/cast.png" alt="cast" width="700"/>

* We can also know more about the cast
<img src="images/cast_info.png" alt="cast info" width="700"/>

### Recommended Movies
* Movies similar to the the one searched by the user are recommended.
<img src="images/rec_mov.png" alt="recommended movies" width="700"/>

### User Reviews
<img src="images/reviews.png" alt="user reviews" width="700"/>


<!-- ACKNOWLEGEMENTS -->
### Sources of the datasets 

1. [IMDB 5000 Movie Dataset](https://www.kaggle.com/carolzhangdc/imdb-5000-movie-dataset)
2. [The Movies Dataset](https://www.kaggle.com/rounakbanik/the-movies-dataset)
3. [List of movies in 2018](https://en.wikipedia.org/wiki/List_of_American_films_of_2018)
4. [List of movies in 2019](https://en.wikipedia.org/wiki/List_of_American_films_of_2019)
5. [List of movies in 2020](https://en.wikipedia.org/wiki/List_of_American_films_of_2020)

## Resources used
* [How to build a recommendation engine](https://www.youtube.com/watch?v=D4nXZMnKW4U)
* [Implementation of movie recommendation](https://www.youtube.com/watch?v=A_78fGgQMjM)
* [Recommender Systems](https://builtin.com/data-science/recommender-systems)
