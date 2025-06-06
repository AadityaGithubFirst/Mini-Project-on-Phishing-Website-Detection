# Mini-Project on Phishing Website Detection
## Overview
This repository contains a mini-project focused on detecting phishing websites using machine learning techniques. The goal is to build and evaluate models that can accurately classify a given URL as either legitimate or a phishing attempt, thereby enhancing online security.Problem StatementPhishing attacks remain a significant threat in the digital landscape, leading to data breaches, financial losses, and identity theft. This project addresses the challenge of identifying and mitigating these threats by developing automated detection systems.FeaturesData Preprocessing: Scripts for cleaning and preparing URL datasets.Feature Engineering: Extraction of relevant features from URLs (e.g., URL length, presence of IP address, suspicious characters, domain age, etc.).Machine Learning Models: Implementation and evaluation of various machine learning algorithms for classification.Light Gradient Boosting Machine (LGBM)Long Short-Term Memory (LSTM) Neural NetworksOther traditional machine learning models (as explored in the notebooks)Model Training & Evaluation: Notebooks demonstrating the training process and performance evaluation using metrics like accuracy, precision, recall, and F1-score.Saved Models: Pre-trained Keras models for quick deployment or further experimentation.Technologies UsedPython: The primary programming language.Jupyter Notebook: For interactive development, experimentation, and analysis.Pandas: For data manipulation and analysis.NumPy: For numerical operations.Scikit-learn: For traditional machine learning algorithms and evaluation metrics.TensorFlow/Keras: For building and training deep learning models (LSTM).LightGBM: For gradient boosting models.Installation and SetupTo set up the project locally, follow these steps:Clone the repository:git clone https://github.com/AadityaGithubFirst/Mini-Project-on-Phishing-Website-Detection.git
cd Mini-Project-on-Phishing-Website-Detection
Create a virtual environment (recommended):python -m venv venv
## On Windows
.\venv\Scripts\activate
## On macOS/Linux
source venv/bin/activate
Install the required dependencies:pip install pandas numpy scikit-learn tensorflow lightgbm jupyter
DatasetThe project utilizes a dataset of URLs labeled as either legitimate or phishing. The dataset is provided in a zipped format:phishing_site_urls.zip: Contains the raw URL data used for training and testing.UsageThe project is structured around several Jupyter notebooks, each potentially exploring different aspects or models.Mini Project.ipynb: Likely the main notebook for initial exploration and model building.Mini Project-Copy1.ipynb, Mini Project-Copy2.ipynb: Possible iterations or alternative approaches.Mini Project-LSTM.ipynb: Specifically focuses on the LSTM model implementation.Mini Project_LGBM.ipynb: Specifically focuses on the LightGBM model implementation.To run the notebooks:Start Jupyter Lab/Notebook:jupyter lab
## or
jupyter notebook
Navigate to the project directory and open the desired .ipynb file.Run the cells sequentially to reproduce the analysis, training, and evaluation.Saved ModelsThe repository includes pre-trained Keras models:Mini_Proj.kerasMini_Proj_LSTM.kerasMini_Proj_saved.kerasThese models can be loaded and used for prediction without retraining.from tensorflow.keras.models import load_model

### Example: Load the LSTM model
model = load_model('Mini_Proj_LSTM.keras')

## You can then use this model to make predictions
## predictions = model.predict(your_processed_data)
ContributingContributions are welcome! If you have suggestions for improvements, new features, or bug fixes, please feel free to:Fork the repository.Create a new branch (git checkout -b feature/YourFeature).Make your changes.Commit your changes (git commit -m 'Add some feature').Push to the branch (git push origin feature/YourFeature).Open a Pull Request.LicenseThis project is licensed under the GPL-3.0 License. See the LICENSE file for more details.ContactFor any questions or inquiries, please contact the repository owner.
