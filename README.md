# Movie-Recommender-System


## Overview

This is a **Movie Recommender System** built using **Streamlit** that provides movie recommendations based on user input. The system utilizes a **pre-trained similarity model** and **The Movie Database (TMDb) API** to fetch movie posters for visual appeal.

## Features

- Users can enter a movie title to get **five recommended movies**.
- Fetches **movie posters** using the TMDb API.
- Uses **cosine similarity** for recommendations.
- Built with **Streamlit** for an interactive UI.

## Requirements

Ensure you have the following dependencies installed:

```bash
pip install streamlit pandas requests pickle5
```

## Installation & Usage

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/movie-recommender.git
   cd movie-recommender
   ```
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the Streamlit app:
   ```bash
   streamlit run app.py
   ```

## File Structure

- `app.py`: Main application file containing the Streamlit interface.
- `movie_dict.pkl`: Preprocessed movie dataset stored as a dictionary.
- `similarity.pkl`: Precomputed similarity matrix for movie recommendations.

## How It Works

1. Loads the movie dataset and similarity matrix using `pickle`.
2. User selects a movie from the dropdown menu.
3. The system finds similar movies based on cosine similarity.
4. Fetches the corresponding **movie posters** using TMDb API.
5. Displays the **recommended movies** along with their posters.

## API Usage

The **TMDb API** is used to fetch movie posters. Replace the `api_key` in the code if needed:

```python
url = "https://api.themoviedb.org/3/movie/{}?api_key=YOUR_API_KEY&language=en-US".format(movie_id)
```

## Example Screenshot



## Future Enhancements

- **Improve recommendations** using collaborative filtering.
- **Enhance UI** with better styling and layouts.
- **Add search functionality** instead of a dropdown selection.

## Author

PRAVEER RAJ
## License

This project is licensed under the **MIT License**.

Thanks for reading.
