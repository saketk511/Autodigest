The 🏎️ AutoDigest 🤖 app is a sophisticated tool designed to enhance the way automotive news and articles are consumed by providing concise summaries from multiple sources. Here's a synopsis of its capabilities:

Comprehensive Article Summarization: Users can input up to five URLs of automotive news articles or research papers into the app. AutoDigest leverages advanced natural language processing to digest these extensive pieces, providing users with succinct, insightful summaries. This feature allows users to quickly grasp the essence of multiple articles without having to read through each one in its entirety.

Intelligent Information Retrieval: Utilizing the RetrievalQAWithSourcesChain from LangChain, the app can answer specific questions posed by the user based on the information contained within the provided URLs. This Q&A feature acts like a personalized research assistant, pulling relevant information from the articles to answer queries directly related to the user's interests in the automotive domain.

Cutting-edge AI Technology: At the heart of AutoDigest are state-of-the-art embeddings and vector storage technologies, including OpenAIEmbeddings and FAISS, which enable the efficient handling and processing of text data. This ensures that the summaries and answers provided are not only relevant but also derived from a comprehensive understanding of the content.

Ease of Use and Accessibility: The app is designed with a user-friendly interface, allowing for effortless navigation and interaction. Users can easily input URLs, initiate the processing with a simple click, and receive their summaries and answers within the main dashboard, making it accessible to professionals, enthusiasts, and casual readers alike.

Environmentally Aware: By utilizing dotenv for environment variable management, AutoDigest ensures that sensitive information, such as the OpenAI API key, is securely handled. This aspect underscores the app's commitment to security and responsible AI use, further enhancing user trust and app reliability.


## Installation

1.Clone this repository to your local machine using:

```bash
  git clone https://github.com
```
2.Navigate to the project directory:

```bash
  cd Autodigest
```
3. Install the required dependencies using pip:

```bash
  pip install -r requirements.txt
```
4.Set up your OpenAI API key by creating a .env file in the project root and adding your API

```bash
  OPENAI_API_KEY=your_api_key_here
```
5. Cut the config.toml file copy it inside "C:\Users\User Name\.streamlit".

## Usage/Examples

1. Run the Streamlit app by executing:
```bash
streamlit run main.py

```

2.The web app will open in your browser.

- On the sidebar, you can input URLs directly.

- Initiate the data loading and processing by clicking "Process URLs."

- Observe the system as it performs text splitting, generates embedding vectors, and efficiently indexes them using FAISS.

- The embeddings will be stored and indexed using FAISS, enhancing retrieval speed.

- The FAISS index will be saved in a local file path in pickle format for future use.
- One can now ask a question and get the answer based on those news articles

## Project Structure

- main.py: The main Streamlit application script.
- requirements.txt: A list of required Python packages for the project.
- faiss_store_openai.pkl: A pickle file to store the FAISS index.
- .env: Configuration file for storing your OpenAI API key.