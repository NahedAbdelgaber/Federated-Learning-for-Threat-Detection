# Federated-Learning-for-Threat-Detection

This simulation uses Federated Learning (FL), enabling data centers (simulated as clients) to collaboratively train models without sharing raw data, ensuring privacy preservation. Each data center trains a local model on its own dataset, and only the model updates (weights) are shared with a central server for aggregation, improving model performance while preserving privacy.

Key Features

	•	Client Models: Each client (representing a data center) trains its model locally using its specific data (i.e., data from that particular data center).
 
	•	Model Aggregation: The central server aggregates the local models by averaging their parameters (in this case, feature importances from decision trees).
 
	•	Simplified Setup: The simulation uses 5 clients running in parallel with a decision tree classifier for faster training.
 
	•	Privacy Preservation: Raw data never leaves the local data centers, ensuring that sensitive information remains protected.

Setup

Prerequisites

To run this project, you’ll need the following Python packages:
	•	Flower for federated learning.
 
	•	Scikit-learn for the machine learning model and evaluation.
	•	Pandas for data manipulation.
	•	NumPy for numerical operations.
