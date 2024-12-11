# LLM Interaction Video Game Idea

This project sets up an interaction between two large language models (LLMs) from OpenAI and Claude, with a third model from Google Gemini to evaluate feedback. The models take turns creating a unique and fun but simple video game idea and evaluating it based on simplicity, fun, and ease of implementation.

## How It Works

1. **Create Thing**: One model creates a video game idea based on the collective feedback.
2. **Evaluate Thing**: The other model evaluates the video game idea based on the specified criteria.
3. **Feedback Buffer**: The feedback is added to a buffer.
4. **Evaluate Feedback**: The third model evaluates the feedback for usefulness, summarizing or compressing it as needed.
5. **Update Collective Feedback**: Useful feedback is added to the collective feedback.
6. **Repeat**: The process repeats for a specified number of interactions.

## Setup

1. Clone the repository.
2. Create a `.env` file with your API keys:
    ```
    OPENAI_API_KEY=your_openai_api_key
    CLAUDE_API_KEY=your_claude_api_key
    GEMINI_API_KEY=your_gemini_api_key
    ```
3. Install the required libraries:
    ```bash
    pip install openai requests python-dotenv
    ```
4. Run the Jupyter notebook.

## Customization

- Change the `thing_to_create` variable to specify what the models should create.
- Change the `evaluation_criteria` variable to specify how the creations should be evaluated.

## Example

```python
thing_to_create = "video game idea"
evaluation_criteria = "simplicity, fun, and ease of implementation"