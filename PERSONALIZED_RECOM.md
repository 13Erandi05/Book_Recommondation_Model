# Personalized Book Recommendation System

This script generates personalized book recommendations based on user's liked books and user-book interactions. It utilizes datasets from Goodreads.

## Dataset

You can download the necessary dataset from the following link: [Goodreads Dataset](https://mengtingwan.github.io/data/goodreads#datasets)

### Dataset Files Needed:

- Detailed book graph (~2gb, about 2.3m books): `goodreads_books.json.gz`
- Complete user-book interactions in 'csv' format (~4.1gb): `goodreads_interactions.csv`

Note: Book IDs in the interaction file can be reconstructed by joining on the following two files:

- `book_id_map.csv`

## Usage

1. Ensure you have the required datasets downloaded and saved in the specified locations.
2. Run the script with Python.
3. Replace the `liked_books.csv` dataset with your own liked books dataset for personalized recommendations.

## Dependencies

- pandas
- numpy
- scipy

## How it Works

1. The script reads user's liked books and user-book interaction data.
2. It identifies users who have similar interaction patterns based on book ratings.
3. Based on these similar users' interactions, it recommends books that the user might like.
4. The recommendations are generated based on the number of ratings, average ratings, and similarity scores.

## Example Output

The script generates personalized book recommendations based on the user's liked books and interaction patterns.

## Note

This script is meant for educational purposes and may require modifications for specific use cases.
