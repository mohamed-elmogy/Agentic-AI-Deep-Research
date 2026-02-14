readme: |
  # 🧠 Agentic AI Deep Research System

  An autonomous multi-agent research system that plans searches, gathers information, synthesizes findings into a structured report, and delivers the results via email — all powered by LLM-based agent orchestration.

  This project demonstrates how Agentic AI systems move beyond chat into autonomous execution pipelines.

  ---

  ## 🚀 What This Project Does

  Given a research query, the system:

  1. 🧠 Plans intelligent web searches  
  2. 🔎 Executes searches in parallel  
  3. 📝 Synthesizes results into a structured research report  
  4. 📧 Sends the final report via email  
  5. 📊 Generates trace logs for observability  

  All orchestrated using multi-agent workflows.

  ---

  ## 🏗️ Architecture Overview

      User Query
          ↓
      ResearchManager
          ↓
      Planner Agent → Generates WebSearchPlan
          ↓
      Search Agent(s) → Perform parallel searches
          ↓
      Writer Agent → Generates structured report
          ↓
      Email Agent → Sends final report

  This architecture demonstrates:

  - Agent orchestration
  - Task delegation
  - Async execution
  - Structured output handling
  - Autonomous workflow execution

  ---

  ## 📂 Project Structure

      Agentic-AI-Deep-Research/
      │
      ├── deep_research.py
      ├── research_manager.py
      ├── planner_agent.py
      ├── search_agent.py
      ├── writer_agent.py
      ├── email_agent.py
      └── README.md

  ---

  ## 🧠 Core Components

  ### 🔹 ResearchManager

  Orchestrates the full pipeline:
  - Plans searches
  - Executes parallel search tasks
  - Writes report
  - Sends email
  - Streams progress updates

  Uses asyncio for concurrent execution.

  ---

  ### 🔹 Planner Agent

  Generates a structured WebSearchPlan:
  - Breaks query into multiple search intents
  - Explains reasoning for each search

  ---

  ### 🔹 Search Agent

  Executes web searches based on planned queries.
  Returns summarized search results.
  Runs concurrently for performance.

  ---

  ### 🔹 Writer Agent

  - Synthesizes all search findings
  - Produces structured research output
  - Returns ReportData object with markdown report

  ---

  ### 🔹 Email Agent

  - Converts report to email-ready format
  - Sends final research report
  - Completes workflow autonomously

  ---

  ## ⚙️ Tech Stack

  - Python 3.9+
  - OpenAI Agents SDK
  - GPT Models
  - Asyncio (Concurrent Execution)
  - Structured Outputs
  - Agent Handoffs
  - Tool-Based LLM Workflows
  - Tracing & Observability

  ---

  ## 🔍 Key Concepts Demonstrated

  - Multi-Agent AI Systems
  - Agent Orchestration
  - Autonomous Task Planning
  - Parallel Async Execution
  - LLM-Driven Decision Making
  - Structured LLM Outputs
  - AI Workflow Automation
  - Production-Style Agent Pipelines

  ---

  ## ▶️ How It Works (Execution Flow)

      async for update in ResearchManager().run("Your research query"):
          print(update)

  Pipeline:
  1. Plan searches
  2. Execute searches in parallel
  3. Write structured report
  4. Send report via email
  5. Return markdown report

  ---

  ## 📊 Observability

  Each run generates a trace:

      https://platform.openai.com/traces/trace?trace_id=...

  Enables:
  - Execution inspection
  - Debugging
  - Agent-level visibility

  ---

  ## 🧪 Example Use Case

      Query:
      "Latest advancements in multi-agent AI systems and their business applications"

  Output:
  - Structured research report
  - Synthesized insights
  - Email delivery
  - Execution trace

  ---

  ## 🔐 Environment Setup

      OPENAI_API_KEY=your_key_here

  ---

  ## 📦 Installation

      git clone https://github.com/your-username/Agentic-AI-Deep-Research.git
      cd Agentic-AI-Deep-Research
      pip install -r requirements.txt

  ---

  ## 🎯 Ideal For

  - AI Engineers
  - Applied LLM Engineers
  - Agentic AI Developers
  - Generative AI Researchers
  - Autonomous Systems Engineers

  ---

  ## 🏷️ Keywords

  Agentic AI • Multi-Agent Systems • LLM Orchestration • Async Execution • Autonomous AI Workflows • Structured Outputs • AI Planning Systems • Generative AI • OpenAI Agents SDK

  ---

  ## 👤 Author

  Mohamed Elmogy  
  AI Engineer | LLM Systems | Agentic AI  

  ---

  ## 📜 License

  MIT License
