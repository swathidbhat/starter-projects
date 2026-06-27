# Google Maps Low Reviews

A short data study of user pain points with Google Maps during trip planning. I
wanted to find what frustrates people most when they use Google Maps to plan a
trip, so the notebook pulls the harshest feedback (1-star reviews) and keeps
only the reviews that mention trip-planning topics.

Original date: 2024-04-22.

## What it does

- Fetches recent reviews of the Google Maps Android app from the Google Play
  Store.
- Keeps only the 1-star reviews.
- Filters those down to reviews whose text mentions trip-planning keywords, such
  as `route`, `navigation`, `itinerary`, `offline`, `road trip`, and `detours`.
- Prints the matching reviews and saves them to `trip_reviews_1_star.csv` with
  the review text, score, and date.

## Setup

1. Install Python 3.
2. Install the dependencies:

   ```bash
   pip install google-play-scraper pandas
   ```

   The notebook also installs these in its first cell, so you can skip this step
   if you run every cell.

## Run it

You can run the notebook two ways.

### In a Jupyter notebook

1. Install Jupyter:

   ```bash
   pip install jupyter
   ```

2. Open the notebook and run all cells:

   ```bash
   jupyter notebook "Google Maps Low Reviews - Trip Planning - Py 3.ipynb"
   ```

### From the command line

1. Convert the notebook to a Python script:

   ```bash
   jupyter nbconvert --to script "Google Maps Low Reviews - Trip Planning - Py 3.ipynb"
   ```

2. Run the script:

   ```bash
   python "Google Maps Low Reviews - Trip Planning - Py 3.py"
   ```

## Output

The notebook prints the filtered reviews and writes `trip_reviews_1_star.csv` to
the working directory. Open that file to read the complaints in one place.

## Adjusting the study

- Change the keyword list to focus on a different theme.
- Change `filter_score_with` to pull a different star rating.
- Change `max_reviews` to fetch more or fewer reviews.
