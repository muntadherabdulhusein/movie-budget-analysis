# Movie Industry – What Drives Box Office Revenue?

A practice project in Python, built while following Alex The Analyst's portfolio series. The question: which features of a movie are most related to how much money it makes?

The dataset has about 7,600 movies with budget, gross revenue, votes, IMDb score, genre, company, runtime and release year.

## What I did

- Checked how much data was missing in each column (budget was missing for 28% of the movies)
- Fixed data types and created a clean release year column
- Checked for duplicates
- Plotted budget against gross revenue with a regression line
- Compared Pearson, Kendall and Spearman correlations and made a correlation heatmap

## Results

- **Budget and gross revenue** have the strongest relationship (Pearson correlation **0.74**)
- **Number of votes** is also strongly related to revenue (0.63)
- The **IMDb score** has almost no relationship with revenue (0.19): a good movie doesn't mean a successful one at the box office

## What I would do differently

Missing budgets were filled with 0, which pulls the correlations down a bit. Next time I would drop those rows or fill them in a smarter way.

## Tools

Python, Pandas, NumPy, Matplotlib, Seaborn

## File

- `movie data project with Python .ipynb`: the full analysis with all charts
