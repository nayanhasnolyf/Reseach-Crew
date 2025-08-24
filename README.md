# 🤖 Research Crew AI

A multi-agent research workflow built with CrewAI.
This project sets up a Researcher Agent and a Reporting Analyst Agent to collaborate on research tasks, generating structured reports automatically.

## 🚀 Features

Agent-Oriented Design: Uses CrewAI’s Agent, Task, and Crew abstractions.

Configurable Agents & Tasks: Agents and tasks are defined in YAML (agents.yaml and tasks.yaml) for flexibility.

## Research Workflow:

Researcher Agent → performs topic exploration.

Reporting Analyst Agent → generates structured summaries and outputs to report.md.

## Multiple Execution Modes:

run() → kickoff workflow with inputs.

train() → iteratively train the crew.

replay() → replay from a specific task.

test() → test crew execution with evaluation.

## ⚡ Getting Started
### 1. Install dependencies
```bash
pip install crewai
```

### 2. Run the workflow
```bash
python main.py
```

### 3. This will run the Research Crew with default inputs:
```bash
inputs = {
    "topic": "AI LLMs",
    "current_year": "2025"
}
```
### 4. Train the crew
``` bash
python main.py train 5 training_output.json
```

👉 Trains for 5 iterations and saves results in training_output.json.

### 5. Replay execution
```bash
python main.py replay research_task
```
### 6. Test execution
```bash
python main.py test 3 gpt-4
```
## 🛠️ Customization

Change Agents & Tasks: Edit agents.yaml and tasks.yaml.

Modify Workflow: Adjust process type (sequential or hierarchical) in crew.py.

Add Tools/Knowledge Sources: Extend agents with external APIs or data sources.

## 📑 Example Output

After running the crew, a report.md file will be generated with structured research findings.

## 🤝 Contributing

Feel free to fork this repo, open issues, or submit PRs to enhance functionality.

## 📜 License

MIT License.
## Made By Nayan
