# Movie Recommendation App

This repository contains a Python-based application for movie recommendations using semantic search powered by Sentence Transformers. The app allows users to input a descriptive query (like "heartfelt romantic comedy") and get movie suggestions that best match their criteria. Filters for IMDb scores and vote counts are also included to refine the results.

## Table of Contents

- Features
- Demo
- Installation
- Usage
- [Dataset](https://raw.githubusercontent.com/datum-oracle/netflix-movie-titles/main/titles.csv)
- Technologies Used
- Future Improvements

## Features

- **Semantic Search:** Get movie recommendations by describing the kind of movie you’re in the mood for.
  
- **Advanced Filtering:** Refine your recommendations based on IMDb scores and vote counts.
  
- **Dynamic User Interface:** Easy-to-use interface powered by Streamlit.

## Running the App in Google Colab

Follow these steps to set up and run the app in Google Colab:

**Step 1: Open Google Colab**

- Go to [Google Colab](https://colab.research.google.com/)
- Click on File > New Notebook to create a new notebook.

**Step 2: Install Dependencies**

In the first cell, run the following command to install the required libraries:

!pip install streamlit sentence-transformers chromadb scikit-learn pandas pyngrok

**Step 3: Write the Application Code**

**Step 4: Run the Streamlit App**

**Step 5: Access the App**

After running the above command, you will see a URL similar to https://<random-string>.loca.lt/. Click on this link to open the Streamlit app in your browser.

**Optional: Ngrok Setup**

If you prefer using ngrok instead of localtunnel, follow these steps:

- Sign up for an ngrok account and get your auth token from the [ngrok dashboard](https://dashboard.ngrok.com/get-started/your-authtoken)

- Run the following command to set your auth token:
<pre>
 !ngrok authtoken (your_auth_token)
</pre>

- Replace the localtunnel command with:
<pre>
 !streamlit run app.py & ngrok http 8501
  </pre>
