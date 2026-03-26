Movie Recommendation System:

Project Overview
This project implements a Movie Recommendation System using content-based filtering. It recommends movies based on similarity in features such as genre, overview, keywords, director, and cast. A graphical user interface built using Tkinter allows users to enter a movie name and receive recommendations instantly.

Methodology
Content-Based Filtering
The system recommends movies by computing similarity between movie features.

Steps Involved
Data preprocessing

Feature combination

Text vectorization

Similarity computation

Recommendation generation

Technologies Used
Programming Language
Python 3.x

Libraries Used
Pandas - Data handling

Scikit-learn - Machine learning algorithms

Tkinter - GUI development

Joblib - Model saving and loading

Project Structure
movie-recommender/
movies.csv - Dataset
train_recommender.py - Model training script
app.py - GUI application
movie_model.pkl - Saved model generated after training

Dataset Description
The dataset contains the following columns:

title - Movie name

genre - Movie category

overview - Short description

director - Director name

cast - Main actors

keywords - Important tags

rating - Movie rating

Installation and Setup
Step 1: Install Python
Download and install Python from the official website.

Step 2: Install Required Libraries
Run the following command in terminal or command prompt:

pip install pandas scikit-learn joblib

How to Run the Project
Step 1: Prepare Dataset
Place the movies.csv file in the project folder and ensure that the column names are correct.

Step 2: Train the Model
Run the following command:

python train_recommender.py

This will process the dataset, create the similarity matrix, and save the model as movie_model.pkl.

Step 3: Run GUI Application
Run the following command:

python app.py

A window will open where the user can:

Enter a movie name

Click "Recommend"

View the top 5 similar movies

How It Works (Technical)
Feature Combination
The system combines multiple text fields into one combined column.

Example:
df["combined"] = df["genre"] + " " + df["overview"] + " " + df["keywords"]

Text Vectorization
TF-IDF is used to convert text data into numerical vectors.

Similarity Calculation
Cosine similarity is used to measure similarity between movies. Higher similarity means more relevant recommendations.

Features
Simple and user-friendly GUI

Fast recommendations

Works offline

Scalable with larger datasets

Limitations
Requires exact movie name input

No personalized recommendations

Dataset may be synthetic

Future Enhancements
Add dropdown suggestions for movie names

Integrate movie posters using APIs

Implement collaborative filtering

Deploy as a web application

Conclusion

This project demonstrates how machine learning techniques can be used to build a real-world recommendation system using efficient algorithms and a simple GUI.
