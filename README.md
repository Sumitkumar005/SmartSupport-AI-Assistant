## 🛒 AI Customer Support Agent with Memory

This Streamlit app implements an AI-powered customer support agent for synthetic data generated using GPT-4o. The agent uses OpenAI's GPT-4o model and maintains a memory of past interactions using the Mem0 library with Qdrant as the vector store.

### Features

- Chat interface for interacting with the AI customer support agent
- Persistent memory of customer interactions and profiles
- Synthetic data generation for testing and demonstration
- Utilizes OpenAI's GPT-4o model for intelligent responses

![High-Level Architecture Diagram](./High-Level%20Architecture%20Diagram.svg)

### Getting Started

Follow these steps to set up the project:

1. **Clone the GitHub repository**
   ```bash
   git clone https://github.com/SmartSupport-AI-Assistant/SmartSupport-AI-Assistant.git
  
   ```

2. **Install the required dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Ensure Qdrant is running**
   The app expects Qdrant to be running on localhost:6333. Adjust the configuration in the code if your setup is different.
   ```bash
   docker pull qdrant/qdrant
   docker run -p 6333:6333 -p 6334:6334 \
       -v "$(pwd)/qdrant_storage:/qdrant/storage:z" \
       qdrant/qdrant
   ```

4. **Run the Streamlit App**
   ```bash
   SmartSupport-AI-Assistant.py
   ```

### Usage Examples

- **Interacting with the AI**: Once the app is running, you can start chatting with the AI customer support agent through the provided interface.

### Contributing

Contributions are welcome! If you would like to contribute to this project, please fork the repository and submit a pull request.

### License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.



