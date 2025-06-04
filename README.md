
# OpenAI Chat Application

A simple Python application that demonstrates how to use the OpenAI GPT-4 API to create a conversational chat interface.

## Description

This application uses the OpenAI API to create a chat conversation where the assistant answers questions about historical events. The example demonstrates a multi-turn conversation about the 2020 World Series.

## Features

- Integration with OpenAI's GPT-4 model
- Multi-turn conversation handling
- Environment variable configuration for API key security
- Error handling for missing API credentials

## Setup

### Prerequisites

- Python 3.11+
- OpenAI API key

### Installation

1. Fork this Repl or create a new Python Repl
2. The required dependencies are already configured in `pyproject.toml`:
   - `openai ^1.3`

### Configuration

1. Get your OpenAI API key:
   - Visit [OpenAI Platform](https://platform.openai.com/signup)
   - Create an account or sign in
   - Navigate to "View API Keys" from the top right menu
   - Click "Create new secret key"

2. Set up your API key in Replit:
   - Open the Secrets tool in your Repl (lock icon in the sidebar)
   - Add a new secret with key: `OPENAI_API_KEY`
   - Paste your OpenAI API key as the value

## Usage

Simply click the "Run" button to start the application. The program will:

1. Check for the OpenAI API key
2. Create a chat conversation with GPT-4
3. Display the assistant's response

## Code Structure

- `main.py`: Main application file containing the OpenAI API integration
- `pyproject.toml`: Poetry configuration with dependencies
- `.replit`: Replit configuration file

## Customization

You can modify the conversation by editing the `messages` array in `main.py`:

```python
messages=[{
    "role": "system",
    "content": "You are a helpful assistant."
}, {
    "role": "user", 
    "content": "Your question here"
}]
```

## API Usage

This application uses OpenAI's Chat Completions API with the GPT-4 model. Make sure you have sufficient credits in your OpenAI account to run the application.

## License

This project is open source and available under the MIT License.

## Support

If you encounter any issues:
1. Ensure your OpenAI API key is correctly set in the Secrets tool
2. Check that you have sufficient OpenAI API credits
3. Verify your internet connection

For more information about the OpenAI API, visit the [OpenAI Documentation](https://platform.openai.com/docs).
