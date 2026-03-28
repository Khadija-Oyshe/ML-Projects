#  Movie Recommender System (Content-Based)

Can data predict your next favorite movie? This project implements a recommendation engine that suggests movies similar to a user's choice by analyzing metadata like genres, keywords, cast, and crew using Natural Language Processing (NLP).

##  Recruiter Highlights
- **Vector Space Modeling:** Transformed raw text data into high-dimensional vectors using `CountVectorizer` to measure document similarity.
- **Mathematical Approach:** Implemented **Cosine Similarity** to calculate the distance between movie vectors, ensuring accurate topical recommendations.
- **Data Engineering:** Performed extensive data cleaning, including literal evaluation of stringified lists and "stemming" to reduce word redundancy (e.g., 'actor' and 'actors' treated as the same).

##  Technical Toolkit
- **Algorithm:** Content-Based Filtering via Cosine Similarity.
- **NLP Techniques:** Stemming (using NLTK), Bag-of-Words, and Text Vectorization.
- **Libraries:** Scikit-Learn, Pandas, Numpy, NLTK.
- **Dataset:** TMDB 5000 Movies Dataset.

##  How it Works
1. **Feature Tagging:** Merged 'overview', 'genres', 'keywords', 'cast', and 'crew' into a single "tags" column.
2. **Text Normalization:** Applied stemming to consolidate similar root words.
3. **Similarity Mapping:** Generated a 5000x5000 similarity matrix to compare every movie against each other.
4. **Recommendation Engine:** A custom function that fetches the top 5 closest neighbors for any given movie title.

##  Example Result
Input: "Bambi"
Recommendations:
1. Naturally Native
2. 30 Nights of Paranormal Activity...
3. The Brave Little Toaster
4. The Jungle Book
5. The Lion King