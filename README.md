# Book Recommendation System

A collaborative filtering experiment in `collaborative_filtering.ipynb`. The notebook uses Goodreads interactions and book metadata to find readers with overlapping preferences and rank books they liked.

## Run the notebook

```bash
git clone https://github.com/tabithaz/Book-Recommendation.git
cd Book-Recommendation
python -m pip install pandas numpy scipy scikit-learn jupyter
jupyter notebook collaborative_filtering.ipynb
```

Place `liked_books_full.csv`, `book_id_map.csv`, `goodreads_interactions.csv`, and `books_titles.json` beside the notebook before running it. These datasets are **not included** in this repository; the first notebook cell links to the source downloads. The notebook cannot run without them.
