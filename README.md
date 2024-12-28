# Personalized Recommendation System

## Overview
The **Personalized Recommendation System** is a web-based application designed to suggest similar products based on user input. Using **cosine similarity**, it ranks products by analyzing user interactions, ratings, and reviews. This system provides an intuitive way for users to explore related products by simply inputting a product name.

---

## Features
- **Content-Based Recommendations**: Suggests similar products based on tags and descriptions.
- **Popularity-Based Ranking**: Incorporates ratings and review counts to rank products.
- **Interactive Web Interface**: Simple and user-friendly interface for input and displaying recommendations.

---

## How It Works
1. **Input**: Users provide a product name.
2. **Processing**:
   - Cosine similarity is computed between the input product and others in the dataset using TF-IDF vectorization.
   - Recommendations are ranked based on similarity scores and product popularity (ratings and reviews).
3. **Output**: A list of recommended products, including:
   - Product Name  
   - Brand  
   - Ratings  
   - Review Count  
   - Product Image  

---

## Technologies Used
- **Backend**: Python with Flask
- **Frontend**: HTML, CSS, Bootstrap
- **Database**: MySQL
- **Libraries**:
  - `pandas` (data manipulation)
  - `scikit-learn` (vectorization and similarity computation)
  - `SQLAlchemy` (database integration)

---

## Installation and Setup

### Prerequisites
- Python 3.7 or higher
- MySQL
- Required Python libraries:
  ```bash
  pip install -r requirements.txt
  
---

## Project Structure
 ```bash
personalized-recommendation-system/
├── static/               # Static files (CSS, JS, images)
├── templates/            # HTML templates
├── models/               # Dataset and preprocessed data files
├── app.py                # Main Flask application
├── requirements.txt      # Python dependencies
├── README.md             # Project documentation
└── database/             # Database schema and configuration
