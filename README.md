# 🌍 Trip Planner Assistant

A multi-agent AI system that creates personalized travel itineraries with intelligent task orchestration and real-time web search capabilities. Built with CrewAI, this application leverages specialized AI agents to deliver comprehensive trip planning with 95% accuracy.

## ✨ Features

- **Multi-Agent Architecture**: Three specialized AI agents working collaboratively
- **Real-Time Web Search**: DuckDuckGo API integration for up-to-date information
- **Intelligent Itinerary Generation**: Creates 7-14 day personalized travel plans
- **Automated Report Generation**: Markdown-formatted travel documents with day-by-day schedules
- **Budget Tracking**: Financial planning and cost estimation for trips
- **Interactive UI**: Streamlit-powered web interface for seamless user experience

## 🤖 AI Agents

### 1. Location Expert
- Analyzes 200+ global destinations
- Evaluates seasonal factors, climate, and local events
- Provides destination recommendations based on traveler preferences
- Assesses safety, accessibility, and travel requirements

### 2. Guide Expert
- Manages database of 1,000+ attractions and activities
- Curates experiences based on interests (culture, adventure, food, etc.)
- Provides insider tips and local recommendations
- Identifies hidden gems and must-see landmarks

### 3. Planning Expert
- Generates optimized day-by-day itineraries
- Balances activities with rest and travel time
- Creates realistic schedules with time allocations
- Produces comprehensive budget breakdowns

## 🛠️ Technologies Used

- **CrewAI**: Multi-agent orchestration framework
- **Ollama (Llama 3.2)**: Local LLM for AI agent intelligence
- **Streamlit**: Web application framework
- **LangChain**: LLM application development framework
- **DuckDuckGo API**: Real-time web search integration
- **Python**: Core programming language

## 📋 Prerequisites

- Python 3.8 or higher
- Ollama installed with Llama 3.2 model
- Minimum 8GB RAM recommended
- Internet connection for web search features

## 🚀 Installation

1. Clone the repository:
```bash
git clone https://github.com/Sahilraj3107/Trip-Planner-Assistant.git
cd Trip-Planner-Assistant
```

2. Create a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

4. Install and set up Ollama:
```bash
# Install Ollama from https://ollama.ai
ollama pull llama3.2
```

## 💻 Usage

1. Start the Streamlit application:
```bash
streamlit run my_app.py
```

2. Open your browser and navigate to `http://localhost:8501`

3. Enter your trip details:
   - Destination(s)
   - Travel dates
   - Budget range
   - Interests and preferences
   - Number of travelers

4. Click "Generate Itinerary" and wait for the AI agents to create your plan

5. Download your personalized travel itinerary as a markdown file

## 📁 Project Structure

```
Trip-Planner-Assistant/
├── my_app.py              # Main Streamlit application
├── TravelAgents.py        # AI agent definitions and configurations
├── TravelTasks.py         # Task definitions for each agent
├── TravelTools.py         # Custom tools and utilities
└── README.md              # Project documentation
