# Google ADK Development Project

A collection of AI agents built with Google's Agent Development Kit (ADK), demonstrating various agent architectures and capabilities.

## 📚 Overview

This project showcases different agent architectures and their applications using Google's ADK:

- Multi-agent systems for tutoring and complex tasks
- Sequential processing for code generation and review
- Parallel agents for research and analysis
- Cloud-based translation and deployment services

## ⚠️ Important Prerequisites

Before running this project, ensure you have:

1. A Google Cloud Platform account with billing enabled
2. Google ADK access and API key
3. Python 3.7 or higher installed
4. Git installed on your system
5. (Optional) OpenAI API key for enhanced capabilities

## 🚀 Quick Start

```bash
# Clone the repository
git clone https://github.com/yourusername/google_adk_dev.git
cd google_adk_dev

# Create and activate virtual environment (recommended)
python -m venv venv
# On Windows:
.\venv\Scripts\activate
# On Unix or MacOS:
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt

# Set up your configuration (see Setup & Requirements section)
# Then run the main multi-agent tutor system:
streamlit run multi_agents_agents_as_tools.py
```

For detailed setup instructions, see the [Setup & Requirements](#%EF%B8%8F-setup--requirements) section.

## 🤖 Components

### Primary Agents

- [`multi_agents_agents_as_tools.py`](multi_agents_agents_as_tools.py) - Tutor bot with Math, Spanish, and Search capabilities
- [`multi-agents/multi_agents_subagents.py`](multi-agents/multi_agents_subagents.py) - Hybrid agent system with dynamic routing

### Processing Systems

- [`sequential_agent.py`](sequential_agent.py) - Code generation pipeline with auto-review
- [`research_parallel_agent.py`](research_parallel_agent.py) - Parallel research processor
- [`loopagent.py`](loopagent.py) - Document writing and improvement system

### Cloud & Deployment Tools

- [`Translate_remote_agent.py`](Translate_remote_agent.py) - Multi-language translation service
- [`deploy_agent.py`](deploy_agent.py) - Cloud deployment manager
- [`agent_management_cli.py`](agent_management_cli.py) - Agent management CLI
- [`multi_tool_agent/agent.py`](multi_tool_agent/agent.py) - Core agent utilities

## ⚙️ Setup & Requirements

### System Requirements

- Python 3.7+
- Google Cloud Platform account
- OpenAI API access (optional)

### Required APIs

- Google ADK (core framework)
- Vertex AI (cloud features)
- Google Search (research agent)
- OpenAI (optional, enhanced capabilities)

### Dependencies

```toml
# Core Dependencies
google-cloud-aiplatform[adk,agent_engines]>=1.48.0
streamlit>=1.24.0
google-generativeai>=0.2.0
python-dotenv>=1.0.0

# Optional Components
openai>=1.0.0  # For GPT-4 integration
vertexai>=0.0.1  # For cloud deployment
nest_asyncio>=1.5.6  # For async operations
```

### Configuration

1. Create `.streamlit/secrets.toml`:

```toml
GOOGLE_API_KEY = "your-google-api-key"
OPENAI_API_KEY = "your-openai-api-key"  # Optional
```

2. For cloud features, set up GCP service account

## 🔧 Key Features

### Multi-Agent Systems

- Specialized agents for Math, Spanish, and Search
- Real-time web search integration
- Content filtering and guardrails
- Dynamic agent configuration

### Processing Pipeline

- Code generation and review
- Research synthesis
- Document improvement
- Progress tracking

### Cloud Services

- Multi-language translation
- Remote deployment
- Agent management
- Resource optimization

## 🛠️ Technology Stack

- **Core Framework**: Google ADK
- **Language Models**: Gemini 2.0 Flash, GPT-4 (optional)
- **Frontend**: Streamlit
- **Cloud Platform**: Vertex AI
- **Agent Types**: Sequential, Parallel, Loop, LLM

## 🔒 Security & Monitoring

### Security Features

- Secure API key management
- Session-based state management
- Input validation
- Content filtering

### Monitoring

- Event logging
- Performance metrics
- Error handling
- Tool execution tracking

## 👥 Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## 📄 License

This project is licensed under the terms provided in the LICENSE file.
