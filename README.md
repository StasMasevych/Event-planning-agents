# Event Plan Agents

A Python-based autonomous agent system that automates event planning using CrewAI. This project demonstrates how multiple specialized agents can collaborate to find venues, manage logistics, and promote events with minimal human intervention.

## 🚀 Features

- **Agentic Event Planning Pipeline**: Multiple agents (Venue Coordinator, Logistics Manager, Marketing Agent) work together to complete event planning tasks.
- **Automated Web Research**: Agents search the web and extract relevant, credible information for venues and logistics.
- **Task Coordination**: Each agent specializes in a key aspect of event management, passing results as needed.
- **Modular & Extensible**: Add or modify agents for custom workflows.
- **Environment Configurable**: API keys and settings via `utils.py` or environment variables.

## 🧩 Main Agents

- **Venue Coordinator**: Finds and books a suitable venue based on event requirements. Outputs details to `venue_details.json`.
- **Logistics Manager**: Arranges catering and equipment for the event. Confirms logistics arrangements.
- **Marketing and Communications Agent**: Markets the event and communicates with participants. Outputs a marketing report to `marketing_report.md`.

## 🏗️ How It Works

1. **Setup**: Configure your API keys in `utils.py` or as environment variables.
2. **Run the App**: Execute `main.py` to start the agent workflow.
3. **Agent Collaboration**: Agents work together to plan and coordinate the event.
4. **Output**: Generates venue details (`venue_details.json`), logistics confirmations, and a marketing report (`marketing_report.md`).

## 📦 Installation

```bash
git clone <repo-url>
cd event-plan-agents
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

## ⚙️ Usage

1. Set up your API keys in `utils.py` or as environment variables.
2. Run the main script:
   ```bash
   python main.py
   ```
3. Edit `main.py` to customize event details, agent tasks, or workflow.

## 📝 Example

```
$ python main.py
[VenueCoordinator] Searching for venues in London...
[LogisticsManager] Arranging catering and equipment...
[MarketingAgent] Promoting the event...
Output saved to: venue_details.json, marketing_report.md
```

## 🛠️ Customization

- Add new agents in `main.py` or separate files.
- Modify agent logic for your needs.
- Integrate with other APIs for more capabilities.

## 📚 Dependencies

- Python 3.8+
- CrewAI (or your agent framework)
- crewai_tools, pydantic, and other packages in `requirements.txt`

## 🤝 Contributing

Pull requests are welcome! For major changes, open an issue first to discuss what you want to change.

---
Feel free to modify or extend the agents for your own event planning needs!
