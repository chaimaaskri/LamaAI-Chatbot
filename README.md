# LamaAI-Chatbot with Streamlit
🦙💬 Build a highly interactive and scalable AI chatbot with Llama 2 model using Streamlit and Replicate API.

## Overview
The LamaAI-Chatbot leverages the latest Llama 2 models to provide engaging conversations. By using Streamlit as the web framework and Replicate for model hosting, this chatbot application is easy to set up, deploy, and interact with. Whether you're a developer or an AI enthusiast, this app offers a fun way to experiment with state-of-the-art AI models.

## Features
- 🎤 **User Inputs**: Type custom messages to interact with the assistant.
- 🔧 **Model Selection**: Choose between Llama 2 7B, 13B, or 70B parameters for different levels of response complexity.
- 🔄 **Real-Time Responses**: Instant AI-generated responses from the selected Llama model based on the input prompt.
- 🛠 **Adjustable Parameters**: Fine-tune settings for temperature, top_p, and max_length to alter response style and length.
- 🔄 **Session Chat History**: Easily keep track of messages exchanged in the same session with the option to clear chat history.
- 🔐 **Replicate API Authentication**: Securely add and authenticate your Replicate API token to interact with hosted models.

## Installation
1. **Clone the repository:**
    ```bash
    git clone https://github.com/chaimaaskri/LamaAI-Chatbot.git
    ```

2. **Install the required dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

3. **Set up Replicate API Token:**
    To use Llama 2 models, create an account on Replicate ([https://replicate.com/](https://replicate.com/)) and obtain your API Token. Enter the token in the Streamlit sidebar when prompted.

4. **Run the app:**
    Once your environment is set up, you can start the application by running:
    ```bash
    streamlit run main.py
    ```
    Visit the URL provided to interact with the chatbot directly on your browser.

## Usage
- **Model Selection**: Choose a model from the sidebar: Llama 2 7B, Llama 2 13B, or Llama 2 70B.
- **Adjust Settings**: Customize the chatbot response style with the sliders for temperature, top_p, and max_length.
- **Interact**: Enter a text prompt in the provided chat input and receive a response from the Llama model.
- **Clear History**: Use the "Clear Chat History" button to reset the conversation and start fresh.

## Code Walkthrough
- **Streamlit Setup**: We initialize the Streamlit app with a page title and sidebar for settings and user inputs.
- **Replicate Integration**: The app integrates with Replicate to call the API for Llama 2 models.
- **Session State**: Chat history is stored in `st.session_state` to maintain messages during the session.
- **Chat Output**: A dynamic chat UI is created, and responses are displayed in real-time.
- **User-Provided Prompt**: We capture input from the user and call Llama 2's API to generate a response.

## Contributing
Feel free to contribute by submitting pull requests or raising issues if you encounter bugs or suggestions for improvements. Your feedback and contributions are always welcome.
