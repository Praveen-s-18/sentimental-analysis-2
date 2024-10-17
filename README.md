# YouTube Comment Sentiment Analysis

This project is designed to perform sentiment analysis on YouTube video comments, helping content creators gain insights into their audience's reactions. By analyzing the sentiment of comments (positive, negative, or neutral), creators can understand viewer feedback and adjust their content accordingly.

## Features

- **Sentiment Analysis**: Analyze the sentiment of YouTube comments (Positive, Neutral, Negative) using NLP techniques.
- **Comment Insights**: Visualize the distribution of positive, neutral, and negative comments.
- **Interactive Interface**: Users can input any YouTube video link, and the system will extract the comments, analyze them, and return a summary of sentiments.
- **Useful for Content Creators**: Helps creators pinpoint areas of their content that may need improvement by identifying negative comments.

## Technologies Used

- **Python**: Main programming language for building the sentiment analysis logic.
- **Streamlit**: Web app framework to create an interactive UI.
- **Matplotlib**: Visualization of comment sentiment distribution.
- **Google API**: To fetch YouTube comments using the YouTube Data API.
- **NLTK (Natural Language Toolkit)**: Sentiment analysis using VADER lexicon.
- **Regular Expressions**: For extracting YouTube video ID from the input URL.

## How it Works

1. **User Input**: The user pastes a YouTube video URL into the app interface.
2. **Fetch Comments**: The system uses the YouTube API to extract up to 100 comments from the video.
3. **Sentiment Analysis**: Each comment is analyzed using the VADER sentiment analysis tool (from the NLTK library) to determine whether it is positive, neutral, or negative.
4. **Results**: The results are displayed in the form of a bar chart, and an overall prediction is made about whether the video has more positive or negative sentiments.

## Installation

### Prerequisites

- Python 3.x
- A Google API key for YouTube Data API access.

### Setup Instructions

1. Clone this repository:
    ```bash
    git clone https://github.com/your-username/youtube-sentiment-analysis.git
    ```

2. Install the required libraries:
    ```bash
    pip install -r requirements.txt
    ```

3. Set up the YouTube Data API:
   - Get an API key from [Google Developer Console](https://console.developers.google.com/)
   - Replace the `api_key` variable in the code with your own API key.

4. Run the Streamlit app:
    ```bash
    streamlit run app.py
    ```

## Usage

- Paste any valid YouTube video link into the input box.
- Click on the **Predict** button to analyze the sentiment of the comments.
- The system will display the sentiment breakdown in the form of a bar chart (positive, neutral, and negative comments).
- The app will also provide an overall sentiment assessment of the video.

## Example

1. Input a YouTube link.
2. Analyze and view the results:
   - Total number of Positive, Neutral, and Negative comments.
   - Bar chart visualization for easy understanding.
   - An overall summary of whether the video has a positive or negative reception.

## Screenshots

![Sentiment Analysis Result](screenshot.png)

## Contributing

Feel free to submit issues or pull requests. Contributions are always welcome to improve this project!

## License

This project is licensed under the MIT License.
