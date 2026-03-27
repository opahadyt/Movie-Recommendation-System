Movie Recommendation System
GUI-Based Content Recommender using Python, Tkinter, TF-IDF, and Cosine Similarity

Project Description
This project is a GUI-based Movie Recommendation System developed in Python using content-based filtering. The program recommends movies similar to a selected movie by analyzing metadata features such as genres, director, and cast. A simple graphical user interface built with Tkinter allows the user to enter a movie title or select one from a dropdown list and instantly receive the top 5 similar movie recommendations.

The recommendation engine uses TF-IDF (Term Frequency-Inverse Document Frequency) to convert combined movie metadata into numerical feature vectors. Cosine similarity is then used to measure how closely related one movie is to other movies in the dataset. Based on the similarity scores, the system ranks and displays the most relevant movie suggestions.

This project is suitable for academic demonstration, beginner machine learning implementation, and offline desktop execution.

Technical Overview
Recommendation Technique:
- Content-Based Filtering

Core Features Used for Similarity:
- Genres
- Director
- Cast

Machine Learning Concepts Used:
- Text feature combination
- TF-IDF vectorization
- Cosine similarity

Interface:
- Tkinter GUI
- Text input for movie title
- Dropdown selection for movie names
- Recommendation display area

Dataset Information
The project uses a CSV dataset containing 1200 movie records.

Dataset columns:
- movie_name
- year
- imdb_rating
- genres
- director
- cast

Important:
The CSV file must remain in the same folder as the Python file, because the program loads the dataset directly using its filename.

Project Files
Keep these files together in one folder:

- movie_recommender_single_file.py
- movie_dataset_1200.csv

Suggested folder structure:

Movie_recommendor_system/
│
├── movie_recommender_single_file.py
├── movie_dataset_1200.csv
└── README.txt

Requirements
Software required:
- Python 3.x

Python libraries required:
- pandas
- scikit-learn

Tkinter note:
Tkinter is generally included with standard Python installations on Windows. In most cases, no separate installation is required.

Installation Steps
1. Install Python on your system.
2. Open Command Prompt.
3. Install the required dependencies using:

   py -m pip install pandas scikit-learn

4. Wait until installation completes successfully.

How to Store the Files
1. Create a folder on your computer, for example:

   C:\Users\YourName\Movie_recommendor_system

2. Save the Python file `movie_recommender_single_file.py` inside that folder.
3. Save the dataset file `movie_dataset_1200.csv` inside the same folder.
4. Make sure both files are in the same directory before running the program.

How to Run the Program
1. Open Command Prompt.
2. Move into the project folder using the `cd` command.

   Example:
   cd C:\Users\YourName\Movie_recommendor_system

3. Run the program using:

   py movie_recommender_single_file.py

4. If everything is set up correctly, the GUI window will open.

How to Use the Program
1. Launch the program.
2. Enter a movie name in the input field, or select a title from the dropdown list.
3. Click the "Recommend" button.
4. The system will display the top 5 similar movies.
5. Each recommendation includes:
   - Movie name
   - Year
   - IMDb rating
   - Genres
   - Director
   - Cast
   - Similarity score

If the entered movie is not found, the program displays sample movie titles so the user can try again.

How the Program Works
1. The dataset is loaded from the CSV file using Pandas.
2. Required columns are validated.
3. Missing values in text fields are handled.
4. The `genres`, `director`, and `cast` fields are combined into one text feature.
5. TF-IDF vectorization converts the combined text into a numerical matrix.
6. Cosine similarity is computed between all movie entries.
7. When the user selects a movie, the program finds the most similar movies based on similarity scores.
8. The top 5 recommendations are shown in the Tkinter GUI.

Program Highlights
- Simple and user-friendly GUI
- Works offline after setup
- Fast recommendation generation
- Uses real machine learning concepts
- Easy to understand for mini project or academic submission
- Single-file implementation for portability and simplicity

Advantages
- Easy to install and run
- Good for learning recommendation system basics
- Does not require internet connection after setup
- Suitable for demonstration and viva presentation
- Can be extended with additional features

Limitations
- Recommendations are based only on metadata
- No personalized user preference learning
- Dataset is synthetic
- Requires Python and dependencies on the user system
- CSV file and Python file must remain together

Future Improvements
- Use real movie metadata from trusted public datasets
- Add poster images and descriptions
- Add spelling correction for search
- Add autocomplete suggestions
- Convert the program into a standalone executable (.exe)
- Build a web-based version using Flask or Django
- Add collaborative filtering or hybrid recommendation methods

Example Command Summary
Install dependencies:
py -m pip install pandas scikit-learn

Run the project:
py movie_recommender_single_file.py

Conclusion
This Movie Recommendation System demonstrates how machine learning techniques such as TF-IDF and cosine similarity can be applied in a practical desktop application. By combining movie metadata and presenting results through a Tkinter GUI, the project provides an effective and beginner-friendly implementation of a content-based recommender system.

Author
Mohammed Ahad Khan
Registration Number: 25BAS10021
