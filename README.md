# Movie Recommender System

## Project Objectives

The Movie Recommender System project aims to build and evaluate a recommendation model that predicts movie ratings for users based on their historical preferences. This system leverages Singular Value Decomposition (SVD) to provide personalized recommendations and improve user experience.

## Key Features

- **Predictive Modeling:** Utilizes SVD to predict missing ratings in a user-item matrix.
- **Personalized Recommendations:** Provides tailored movie suggestions based on user preferences.
- **Evaluation Metrics:** Assesses model performance using appropriate metrics (e.g., RMSE).

## How to Run the Notebook

1. **Set Up AWS SageMaker:**
   - Ensure you have an AWS account with SageMaker access.
   - Upload the dataset to an S3 bucket.

2. **Clone the Repository:**
   ```bash
   git clone https://github.com/yourusername/movie-recommender.git
   cd movie-recommender
3. Run the Jupyter Notebook:
   
Open SageMaker and navigate to the Jupyter notebook instance.
Open Movie_Recommender.ipynb.
Run the cells sequentially to execute the model training and evaluation.

4. Explanation of the Dataset
The dataset used for training the model includes user ratings for various movies. It is structured as follows:

UserID: Unique identifier for each user.
MovieID: Unique identifier for each movie.
Rating: Rating given by the user to the movie (on a scale from 1 to 5).
The dataset can be found in the data/ directory and is read from an S3 bucket.

5. Instructions for Installing Dependencies
Ensure you have the following Python packages installed:

pandas
numpy
scikit-learn
matplotlib
awscli
You can install the dependencies using pip:
pip install pandas numpy scikit-learn matplotlib awscli

6. Results
The SVD model was trained with the following parameters:

Number of Singular Value Decomposition (SVD) Components: 50
Regularization Parameter: 0.1
The best model achieved a Root Mean Square Error (RMSE) score of 0.85 on the validation set, indicating effective prediction of movie ratings.
