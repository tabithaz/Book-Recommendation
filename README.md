
# Book Recommendation System

A Python-based book recommendation engine that suggests titles tailored to a user’s reading preferences using collaborative filtering and overlap-based user similarity.

## Features
- Personalized recommendations based on user overlap
- Filters to include only users with significant shared book preferences
- Data cleaning and normalization for consistent matching
- Bayesian scoring to prevent bias toward books with few ratings
- Outputs titles, average ratings, Goodreads links, and cover images

## Data Sources
The system uses:
- `liked_books_full.csv` — List of books you have liked or rated highly
- `book_id_map.csv` — Mapping between CSV IDs and Goodreads IDs
- `goodreads_interactions.csv` — Ratings from other Goodreads users
- `books_titles.json` — Metadata for books (title, cover image, Goodreads URL)

## Tech Stack
- Python 3
- Pandas for data manipulation
- NumPy for numerical operations
- Jupyter Notebook for experimentation and visualization

## How It Works
1. Load the liked books file
2. Map internal CSV IDs to Goodreads IDs
3. Identify users with more than 20% overlap in liked books
4. Aggregate and average ratings from those users
5. Apply rating count and average rating thresholds
6. Rank results using a Bayesian average score
7. Display results with links and cover images

## Getting Started

**1. Clone the repository**
```bash
git clone https://github.com/yourusername/book-recommendation.git
cd book-recommendation
````

**2. Install dependencies**

```bash
pip install -r requirements.txt
```

**3. Add data files**
Place the following files in the project folder:

* `liked_books_full.csv`
* `book_id_map.csv`
* `goodreads_interactions.csv`
* `books_titles.json`

**4. Run the project**

```bash
jupyter notebook book_recommender.ipynb
```


