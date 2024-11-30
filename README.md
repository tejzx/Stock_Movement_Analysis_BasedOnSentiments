# StockMovementAnalysisBasedOnSentiments
The Reddit Stock Sentiment Analyzer is a Python-based application that scrapes Reddit posts, analyzes their sentiment, and presents insights through visualizations. It uses a Gradio interface for an interactive and user-friendly experience. Users can input a subreddit name and view sentiment analysis results alongside graphical trends.
Features
Reddit Scraping:
Fetch posts from any specified subreddit using the Reddit API.
Retrieve post metadata (title, content, score, and date).
Sentiment Analysis:
Classify posts into positive or negative sentiments using a trained machine learning model.
Visualizations:
Sentiment distribution bar chart.
Sentiment scores over time line plot.
Text length by sentiment boxplot.
Gradio Interface:
Easy-to-use web-based interface for input and output.
Dynamic generation of sentiment analysis results and visualizations.

Technologies Used
Python: Core programming language.
PRAW: For Reddit API integration.
Scikit-learn: For machine learning and sentiment classification.
Seaborn & Matplotlib: For creating visualizations.
Gradio: For building and deploying the interactive interface.

Setup Instructions
1. Clone the Repository
git clone <repository-url>
cd <repository-folder>
2. Install Dependencies
Create a virtual environment (optional) and install the required Python libraries: pip install -r requirements.txt
3. Configure Reddit API
Create a Reddit Developer account and generate API credentials.
Replace the placeholders in the script with your credentials:
CLIENT_ID = "your_client_id"
CLIENT_SECRET = "your_client_secret"
USER_AGENT = "your_user_agent"
4. Run the Application
Launch the application locally: python app.py
For a public link, use: gr.Interface.launch(share=True)
How to Use
Input: Provide the following in the Gradio interface:
Subreddit name (e.g., stocks).
Number of posts to analyze.
Output:
A table showing the sentiment classification of each post.

Visualizations:
Sentiment distribution.
Sentiment scores over time.
Text length versus sentiment.
Example Screenshots
1. Input Interface

2. Sentiment Distribution

3. Sentiment Scores Over Time

Deployment Options
Hugging Face Spaces:
Create a Hugging Face Space and upload the code along with requirements.txt.
Select the Gradio SDK, and the app will be hosted at a public URL.
Render:
Use Render to deploy the app with more flexible configuration options.
Other Options:
Use Deta or Google Colab for free hosting.
Limitations
Small training dataset may limit model accuracy.
Analysis is dependent on the quality of subreddit discussions.
Visualizations rely on sufficient data from the subreddit.

Future Enhancements
Use a larger, more diverse training dataset for better classification.
Add support for scraping multiple platforms (e.g., Twitter, Telegram).
Introduce dynamic, interactive visualizations with libraries like Plotly.
