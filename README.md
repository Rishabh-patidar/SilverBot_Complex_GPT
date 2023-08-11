# Silver Chatbot Project

Silver Chatbot is a project that combines a FastAPI backend with a React.js frontend to create a user-friendly chatbot interface. The chatbot is powered by OpenAI's GPT model for generating responses.

## Backend (FastAPI)

### Main Files:
- `main.py`: This file contains the FastAPI application setup and API routes for the chatbot.

### Major Functions:
- `answer_me(query: str)`: This route processes user queries, constructs a conversation prompt, and sends it to the GPT model for generating a response. It saves the conversation history and returns the bot's response.
- `get_conversations()`: This route fetches and returns the stored conversation history from the database.
- `del_conversations()`: This route deletes all conversations from the database.

## Frontend (React.js)

### Main Files:
- `Home.js`: This file contains the main chat interface and user interactions.

### Major Functions:
- `handleChange(e)`: Handles user input change in the chat input field.
- `handleSubmit(e)`: Handles user input submission, sends it to the backend, and updates the conversation.
- `handleDelete(e)`: Handles the deletion of conversations and clears the conversation history.
- `handleConversationFetch()`: Fetches and updates the conversation history from the backend.
- `useEffect()`: Fetches the initial conversation history on component mount.

## Database 
The database module (`database.py`) handles interactions with the database for storing and retrieving conversations.

## Installation and Setup
1. Backend: Install required Python packages using `pip install fastapi uvicorn`. Run the backend using `uvicorn main:app --reload`.
2. Frontend: Install dependencies using `npm install` and start the development server with `npm start`.

## Usage
1. Access the chatbot interface at `http://localhost:3000`.
2. Enter your questions in the input field and click "Submit" to receive responses.
3. Click "Delete" to clear conversation history.

## Error
gpt_index named library is changed to lamma_index and its functions are also changed.
