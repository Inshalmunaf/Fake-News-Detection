# Fake News Predictor GUI Project

## Project Setup Instructions

To run this Fake News Prediction application, please follow these steps:

### 1. Prerequisites
Ensure you have Python installed on your system (preferably Python 3.7 or newer). You can download it from python.org.

Ensure pip (Python's package installer) is installed and updated.

### 2. Download Project Files
Download all the project files, including:
* The Python notebook for the GUI: `test_fake_news_project.ipynb`.
* The `requirements.txt` file (provided below).
* The pre-trained model files:
    * `logistic_model.pkl`
    * `Naive_model.pkl`
    * `tfidf_vectorizer.pkl`
    * `lstm_fake_news_model.h5`
    * `tokenizer.pkl`
* Place all these files in the same directory on your computer.

### 3. Create requirements.txt
Create a new text file named `requirements.txt` in the same directory as your Python notebook and model files. Copy and paste the following content into it:

\`\`\`text
numpy
scikit-learn
tensorflow
nltk
joblib
\`\`\`

### 4. Install Required Libraries
* Open a terminal or command prompt.
* Navigate to the directory where you saved the project files (e.g., using the `cd` command).
* Install the necessary Python libraries by running the following command:
    \`\`\`bash
    pip install -r requirements.txt
    \`\`\`
    This command will read the `requirements.txt` file and install all the listed libraries and their dependencies.

### 5. Run the Application
* Once the libraries are installed, you can run the GUI application.
* Open the `test_fake_news_project.ipynb` file in a Jupyter-compatible environment (like VS Code with the Jupyter extension, Jupyter Lab, or Jupyter Notebook).
* Run all the cells in the notebook in order. The Tkinter window containing the GUI should appear.

* **NLTK Data Download:** The first time you run the application from the notebook, it might take a moment to download necessary NLTK data packages (\`punkt\`, \`stopwords\`, \`wordnet\`). This is handled automatically by the script within the notebook. If you encounter issues, ensure you have an active internet connection.

### Troubleshooting
* If you encounter errors related to a specific library, try installing it individually (e.g., \`pip install tensorflow\`).
* Ensure the model files and the \`tfidf_vectorizer.pkl\` / \`tokenizer.pkl\` are in the same directory as the notebook, or that the code correctly points to their location if they are elsewhere. The GUI script expects them in the same directory.
* If you encounter errors like \`NameError: name 'get_ipython' is not defined\` when trying to run parts of the notebook or if you attempt to convert it to a script yourself, it might indicate notebook-specific code (like magic commands) that isn't compatible outside a full Jupyter environment.