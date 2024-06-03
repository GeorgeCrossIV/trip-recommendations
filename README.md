# Trip Recommendation, Similarity Search & Collaborative Filtering

## Introduction

This project aims to develop a trip similarity search feature for travelers using [AstraDB](https://www.datastax.com/products/datastax-astra) and vector embeddings. By leveraging AstraDB's vector database and OpenAI's advanced embedding techniques, we aim to provide personalized travel suggestions based on users' past preferences or trending selections. Additionally, collaborative filtering is integrated to enhance recommendation capabilities beyond vector-based similarity searches, predicting user preferences based on the preferences of others.

## Notebook

You can find the full implementation in the [Trips_Similarity_Search_Vector_Search.ipynb](./Trips_Similarity_Search_Vector_Search.ipynb) notebook.

## Prerequisites

Ensure you have the following before running the notebook:

- [Astra DB](https://www.datastax.com/products/datastax-astra) database with vector enabled (endpoint and token)
- OpenAI API key
- [Kaggle](https://www.kaggle.com/) API key (username and token)

## Project Phases

We will utilize the [Kaggle Travel Dataset (argodatathon2019)](https://www.kaggle.com/competitions/argo-dataathon-2019) to develop our system through the following phases:

1. **Vector Embedding Generation**: Convert travel data into vector embeddings using OpenAI’s models, extracting useful features and transforming them into numerical vectors.

2. **AstraDB Setup**: Configure and deploy AstraDB to store and manage these embeddings efficiently, designing a schema that supports quick retrieval and similarity searches.

3. **Data Insertion**: Populate AstraDB with the preprocessed and embedded travel data.

4. **Similarity Search Implementation**: Develop a querying mechanism in AstraDB to identify and suggest trips that are most similar to a user's input or preferred travel profile.

5. **Collaborative Filtering Implementation**: Integrate collaborative filtering to improve recommendation quality by leveraging both content-based features and user interaction patterns.

6. **Interface and Deployment**: Create a user-friendly interface for travelers to find and explore suggested trips, refining the system based on user feedback.

## Similarity Search Implementation

The core functionality of the trip similarity search system is demonstrated through practical examples:

- **Retrieve a User Profile**: Fetch user data based on a unique identifier (Profile ID).
- **Profile Search by Attributes**: Search for profiles using key factors such as gender, age group, trip destination, and price preferences.
- **Similar Trips from Attributes**: Find trips that align with a set of randomly generated user trip attributes.
- **Natural Language Search**: Use natural language descriptions to find trips that match user preferences.

## Collaborative Filtering Queries - Find Recommended User
Trips

Collaborative filtering leverages user similarity and past interactions to recommend trips, considering the weight of user trips, such as how frequently a user visits a particular location. This approach refines recommendations based on the intensity or frequency of user preferences.

## Project Summary

This notebook details the creation of a trip similarity search system using AstraDB and vector embeddings from OpenAI. Key components include:

- **Vector Embeddings**: Generate embeddings from travel data to capture essential features of each trip.
- **AstraDB Configuration**: Set up and configure [AstraDB](https://www.datastax.com/products/datastax-astra) for efficient storage and retrieval of embeddings.
- **Data Management**: Insert and manage travel data within AstraDB, ensuring integrity and accessibility.
- **Similarity Searches**: Implement search functionalities to find similar trips based on user profiles, specific attributes, and natural language descriptions.
- **User Interface Integration**: Create a user-friendly interface for travelers to interact with the system and receive personalized trip recommendations.

This project showcases how vector databases and AI-driven embeddings can revolutionize personalized travel recommendations, making the process more intuitive and user-centric.
