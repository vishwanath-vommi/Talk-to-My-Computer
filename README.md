# Talk to My Computer

"Talk to My Computer" is a simple Python application that allows users to chat with an AI assistant using text-based prompts. This program is powered by the GPT-3.5-turbo API and is designed to be executed in a Google Colab environment as a `.ipynb` file. Users can enter their questions or messages, and the assistant will respond accordingly.

---

## Features

- **Text-Based Interaction**: Communicate with the assistant using text prompts.
- **API Integration**: Powered by GPT-3.5-turbo for intelligent responses.
- **Exit at Any Time**: Type `bye` or press `Ctrl+C` to end the chat.
- **Error Handling**: Handles API communication errors gracefully.

---

## Requirements

To run this project, you will need:

- Python 3.6 or later (pre-installed in Google Colab)
- Internet connection
- An API key for the GPT-3.5-turbo API via RapidAPI
- Google Colab account

---

## Setup Instructions

1. **Open Google Colab**:
   - Go to [Google Colab](https://colab.research.google.com/).

2. **Create a New Notebook**:
   - Click on "File > New Notebook" to create a new `.ipynb` file.

3. **Copy the Code**:
   - Paste the Python code into a code cell in the Colab notebook.

4. **Add Your API Key**:
   - Replace the placeholder `x-rapidapi-key` in the code with your own RapidAPI key.

5. **Run the Notebook**:
   - Execute the code cells in order to start the program.

---

## Usage

1. Launch the program by running the cell containing the main function.
2. Start chatting by typing your messages in the input prompts.
3. To end the conversation, type `bye`.

### Example Interaction:

```text
Welcome to 'Talk to My Computer'!
Type 'bye' at any time to end the conversation.

You: What is Java?
Compy: Java is a high-level, object-oriented programming language developed by Sun Microsystems in 1995. It is widely used for building enterprise-level applications, web applications, mobile applications, and software development...

You: Thank you!
Compy: You're welcome! How else can I assist you?

You: bye
Compy: Goodbye! Talk to you later.
```

---

## Code Explanation

### API Integration
- The application sends user messages to the GPT-3.5-turbo API endpoint using an HTTPS POST request.
- The response is parsed to extract and display the assistant's message.

### Exit Conditions
- The chat ends when the user types `bye` or presses `Ctrl+C`.
- The program handles `KeyboardInterrupt` to ensure a graceful exit.

---

## Troubleshooting

- **Error Communicating with the API**: Ensure your API key is valid and you have an active internet connection.
- **Invalid Responses**: If the assistant doesn't respond as expected, check if the API service is operational.

---

## Acknowledgments

- OpenAI for GPT-3.5-turbo
- RapidAPI for providing API access
- Google Colab for the notebook environment
