# AI Financial Assistant and Web Playground
This project is a Python-based AI-driven financial assistant and web search playground. It leverages various tools and APIs for financial data retrieval, web searches, and interactive agent-based exploration.
## Features
### AI Agents
1. **Web Search Agent**:
   - Uses DuckDuckGo for web searches
   - Ensures source inclusion in responses
   - Provides information in a structured and markdown-friendly format
2. **Finance AI Agent**:
   - Utilizes YFinance to fetch:
     - Stock prices
     - Analyst recommendations
     - Stock fundamentals
     - Latest company news
   - Displays data in easy-to-read tables
3. **Multi-Agent Team**:
   - Combines the Web Search and Finance AI Agents
   - Delivers comprehensive results for queries requiring both web search and financial data
### Interactive Playground
- A user-friendly interface for experimenting with the AI agents
- Built using the Playground component of the Phi framework
- Includes the ability to run, test, and interact with agents in real time
## Installation
### Prerequisites
Ensure you have the following installed:
- Python 3.8 or above
- pip (Python package manager)
### Steps
1. Clone the repository:
```bash
git clone https://github.com/your-username/ai-financial-assistant.git
cd ai-financial-assistant
```
2. Install the required dependencies:
```bash
pip install -r requirements.txt
```
3. Create a `.env` file in the project root directory and add your API keys:
```makefile
OPENAI_API_KEY=your_openai_api_key
PHI_API_KEY=your_phi_api_key
```
## Usage
### Running the Financial Agent
The `financial_agent.py` script demonstrates the usage of the Finance AI Agent and the Multi-Agent Team:
```bash
python financial_agent.py
```
### Running the Playground
The `playground.py` script launches an interactive web-based playground:
```bash
python playground.py
```
Visit the provided URL in your browser to explore the playground.
### Example Query
For financial analysis:
* Query: "Summarize analyst recommendations and share the latest news for NVDA."
* Output: Tabular data with stock prices, recommendations, and related news.
## Project Structure
```bash
.
├── financial_agent.py    # Script to run financial agent tasks
├── playground.py        # Script to launch the web-based playground
├── requirements.txt     # List of dependencies
├── .env.example        # Example environment file for API keys
```
## Requirements
The following Python libraries are used:
* `phidata`: For agent creation and interaction
* `python-dotenv`: To manage environment variables
* `yfinance`: For financial data
* `duckduckgo-search`: For web search capabilities 
* `fastapi` and `uvicorn`: For serving the playground web app
* `groq`: For Groq-based AI model integration
* `openai`: To integrate OpenAI models
## Future Enhancements
* Add more agents for diversified tasks
* Enhance the user interface of the playground
* Expand financial tools to include cryptocurrency and forex analysis
## License
This project is licensed under the MIT License.
## Contributions
Contributions are welcome! Please submit a pull request or open an issue for suggestions or bug reports.
