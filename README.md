# tau-prolog_movie-recommendation-system-
AI-Powered Movie Recommender (Expert System)

A 100% Client-Side Expert System for movie recommendations, built using Prolog for logical inference and Tau Prolog for seamless web browser integration.
 Preview



 Features

Serverless Architecture: The entire AI logic runs completely inside the browser using JavaScript and Tau Prolog. Zero backend required!

Declarative Knowledge Base: Contains a rich dataset of movies mapped via Prolog facts (film/10).

Advanced Filtering: Query movies by Director, Year, Rating, or Genre using custom logical rules.

Personalized Recommendations: Uses deductive logic (recommend/2) to match users with movies based on their specific genre preferences.

Modern UI: A sleek, cinematic dark-themed interface built with HTML/CSS that replaces the traditional SWI-Prolog console.

Tech Stack

Logic Engine: Prolog (Facts, Rules, Recursion, Lists).

Web Middleware: Tau Prolog (JavaScript Prolog Interpreter).

Frontend: HTML5, CSS3, Vanilla JavaScript.




2. Logical Rules (Inference):

% Find High-rated movies
high_rating(Movie) :- rating(Movie, Value), Value >= 8.0.

% Personalized Recommendation Engine
likes('Ahmed', 'scifi').
recommend(Person, Movie) :- likes(Person, Genre), genre(Movie, Genre).


3. Advanced List Processing (Recursion):

% Count total number of movies recursively
count_movies([], 0).
count_movies([_|Tail], Count) :- count_movies(Tail, TailCount), Count is TailCount + 1.


