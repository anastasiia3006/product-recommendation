Product Recommendation System for E-Commerce
Project Overview

This project demonstrates the creation of a Product Recommendation System for an e-commerce platform. It includes customer clustering, collaborative filtering for recommendations, data visualization, and deployment of an API using Flask and ngrok. The system helps businesses better understand customer behavior and provide personalized product recommendations to enhance the user experience and boost sales.
Features

  Data Preprocessing:
        Handling missing and duplicate data.
        Merging multiple datasets for analysis.
    Customer Clustering:
        Using K-Means to segment customers into groups based on their purchase behavior.
        Optimal cluster selection with the Elbow Method.
    Recommendation System:
        Collaborative filtering using K-Nearest Neighbors (KNN).
        Real-time recommendations based on similar customer behavior.
    Visualization:
        Analysis of product popularity and customer segments.
        Dimensionality reduction with PCA for clustering visualization.
    API Deployment:
        Flask-based API for external applications to query the recommendation system.
        Exposed using ngrok for easy testing and integration.

Installation

  Clone the repository:

git clone https://github.com/your_username/product-recommendation-system.git

Navigate to the project directory:

cd product-recommendation-system

Install dependencies:

  pip install -r requirements.txt

Usage

  Run the Project in Google Colab:
        Upload the project files to Google Colab.
        Ensure all required libraries are installed.

  Start the Flask API:
        Run the script in Google Colab.
        The ngrok public URL will be generated. Use it to access the API.

  API Endpoints:
        /recommend (GET):
            Parameters:
                customer_name: Name of the customer (e.g., Bharat).
                num_recommendations: Number of recommendations to return (default is 5).
            Example:

https://<ngrok-url>/recommend?customer_name=Bharat&num_recommendations=5

Output:

            {
                "customer_name": "Bharat",
                "recommendations": [
                    {"product": "Product A", "score": 95},
                    {"product": "Product B", "score": 88}
                ]
            }

Results

  Clustering successfully grouped customers into segments, allowing for targeted marketing.
  Recommendations provided relevant products based on similar customers’ behavior.
  API integration enabled external applications to use the recommendation engine.
