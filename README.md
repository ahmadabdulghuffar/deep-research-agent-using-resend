🔍 Deep Research AI Agent System
An intelligent multi-agent research system that conducts parallel web searches, synthesizes information, and delivers comprehensive reports via email.

Built by Ahmad Abdul Ghaffar | AI Agent Engineer | ahmadabdulghuffar@gmail.com


🎯 What This Does
This AI system automates the research process by:

Planning - Generates strategic search queries based on your question
Searching - Executes parallel web searches for faster results
Analyzing - Synthesizes information from multiple sources
Writing - Creates comprehensive, well-structured reports
Delivering - Sends formatted HTML reports directly to your email
Example:
You ask: "What are the latest developments in AI agent frameworks?"
The system researches, analyzes, and emails you a detailed report in minutes.

🏗️ System Architecture
This is a multi-agent orchestration system with specialized agents:

Agent Structure
User Query
    ↓
Planner Agent → Creates search strategy
    ↓
Search Agents → Execute parallel web searches (AsyncIO)
    ↓
Research Manager → Coordinates workflow
    ↓
Writer Agent → Synthesizes findings into report
    ↓
Email Agent → Delivers HTML report
Key Components
File	Purpose
planner_agent.py	Generates strategic search queries using structured outputs
search_agent.py	Performs web searches and extracts relevant data
research_manager.py	Orchestrates agent workflow and data flow
writer_agent.py	Creates comprehensive research reports
email_agent.py	Sends formatted reports via Resend API
deep_research.py	Main execution pipeline with Gradio UI
⚡ Key Features
1. Parallel Processing
Uses AsyncIO for concurrent web searches
Significantly faster than sequential searching
Handles multiple queries simultaneously
2. Structured Outputs (Pydantic)
Ensures consistent data format between agents
Type-safe agent communication
Validates data at every step
3. Modular Architecture
Each agent has single responsibility
Easy to modify or extend
Scalable for additional features
4. Smart Research Planning
AI-powered query generation
Strategic search term selection
Reason-based search justification
5. Professional Delivery
Clean HTML email formatting
Well-structured reports
Automatic email delivery via Resend
🛠️ Tech Stack
Core Technologies:

Python - Primary language
OpenAI GPT-4 - LLM for intelligent agents
Gradio - Web UI interface
AsyncIO - Parallel search execution
Pydantic - Structured data validation
Resend API - Email delivery
Key Libraries:

agents - Agent orchestration framework
dotenv - Environment variable management
requests / aiohttp - Web searching
📋 How It Works
Step-by-Step Process
1. User Input

"Research the impact of climate change on real estate values"
2. Planner Agent Generates 3 strategic search queries:

json
{
  "searches": [
    {
      "reason": "Need current flood risk data",
      "query": "climate change flood zones property values 2025"
    },
    {
      "reason": "Historical price trends",
      "query": "real estate climate risk pricing trends"
    },
    {
      "reason": "Future predictions",
      "query": "climate change real estate market forecast"
    }
  ]
}
3. Search Agents (Parallel) Execute all 3 searches simultaneously using AsyncIO

4. Writer Agent Synthesizes findings into comprehensive report with:

Executive summary
Key findings
Data sources
Conclusion
5. Email Agent Delivers formatted HTML report to user's inbox

🚀 Setup & Installation
Prerequisites
Python 3.8+
OpenAI API key
Resend API key (with verified domain)
Installation
bash
# Clone the repository
git clone https://github.com/yourusername/deep-research-agent.git
cd deep-research-agent

# Install dependencies
pip install -r requirements.txt

# Create .env file
cp .env.example .env
Environment Variables
Create a .env file:

properties
OPENAI_API_KEY=sk-your-key-here
RESEND_API_KEY=re-your-key-here
Run the Application
bash
python deep_research.py
Then open the Gradio interface in your browser.

💡 Use Cases
Business Intelligence
Market research
Competitor analysis
Industry trend tracking
Real Estate
Property market analysis
Climate risk assessment
Neighborhood research
Investment Research
Company due diligence
Sector analysis
Risk evaluation
Academic Research
Literature reviews
Topic exploration
Source gathering
🎓 What I Learned Building This
Technical Skills
✅ Multi-agent orchestration
✅ Parallel processing with AsyncIO
✅ Structured outputs with Pydantic
✅ Email automation with Resend
✅ Gradio UI development
✅ Modular system architecture

AI Engineering Concepts
✅ Agent communication protocols
✅ Workflow orchestration
✅ Tool calling and function schemas
✅ LLM prompt engineering
✅ Data normalization across agents

🔮 Future Enhancements
Planned Features:

 Multi-model support (Claude, Gemini, etc.)
 Source citation tracking
 PDF report generation
 Custom report templates
 API endpoint for integration
 Data caching for faster repeated queries
 Advanced filtering and relevance scoring
📊 System Performance
Average Research Time:

Simple queries: 30-60 seconds
Complex queries: 1-3 minutes
Parallel vs Sequential:

3 searches sequentially: ~90 seconds
3 searches in parallel: ~30 seconds
Performance gain: 3x faster
🤝 About the Developer
Ahmad Abdul Ghaffar
AI Agent Engineer | Marketing Growth Expert

Background:

11× sales growth in EV marketing
Transitioning from Marketing to AI Engineering
Specializing in Agentic AI Systems
Skills:

Python, LangChain, OpenAI API
Multi-agent orchestration
Marketing automation
Business process automation
Connect:


💼 LinkedIn: linkedin.com/in/ahmadabdulghaffar
📧 Email: ahmadabdulghuffar@gmail.com
💼 Custom Development
Need a custom AI agent system for your business?

I build intelligent automation solutions:

Research automation agents
Customer support agents
Marketing automation systems
Data analysis pipelines
Custom AI integrations


📧 Contact: ahmadabdulghuffar@gmail.com

📄 License
This project is for educational and demonstration purposes.

🙏 Acknowledgments
Built as part of "The Complete Agentic AI Engineering Course (2025)" by Ed Donner.

Special thanks to the AI engineering community for resources and inspiration.

⭐ If you find this useful, star the repo and reach out for collaboration!

