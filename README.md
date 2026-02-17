## Problem

Planning multi-day trips requires aggregating information across destinations, attractions, budgets, and time constraints. Manual planning is time-consuming and often results in unrealistic or incomplete itineraries.

## Solution

This project implements a **multi-agent AI system** that decomposes trip planning into specialized reasoning tasks and coordinates them using intelligent agent orchestration.  
The system combines **LLM-based reasoning** with **real-time web search** to generate constraint-aware, personalized travel itineraries.

The focus of this project is on **agent collaboration, task decomposition, and orchestration**, rather than single-prompt itinerary generation.

## Key Design Decisions & Trade-offs

- **Multi-Agent over Single LLM Prompt**: Improves modularity and allows independent reasoning for destinations, attractions, and scheduling.
- **Real-Time Web Search**: Ensures recommendations remain relevant and up-to-date.
- **Local LLM via Ollama**: Reduces inference cost and improves iteration speed, with acceptable trade-offs in model accuracy.
- **Sequential Task Execution**: Prevents conflicting recommendations and reduces redundant web queries.


## ✨ Features

- **Multi-Agent Architecture**: Three specialized AI agents working collaboratively
- **Real-Time Web Search**: DuckDuckGo API integration for up-to-date information
- **Intelligent Itinerary Generation**: Creates 7-14 day personalized travel plans
- **Automated Report Generation**: Markdown-formatted travel documents with day-by-day schedules
- **Budget Tracking**: Financial planning and cost estimation for trips
- **Interactive UI**: Streamlit-powered web interface for seamless user experience

## 🤖 AI Agents

### 1. Location Expert
- Analyzes  global destinations
- Evaluates seasonal factors, climate, and local events
- Provides destination recommendations based on traveler preferences
- Assesses safety, accessibility, and travel requirements

### 2. Guide Expert
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

