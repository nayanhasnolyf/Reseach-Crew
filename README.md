<<<<<<< HEAD
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
=======
# Research Crew

Welcome to the Research Crew project, powered by [crewAI](https://crewai.com). This template is designed to help you set up a multi-agent AI system with ease, leveraging the powerful and flexible framework provided by crewAI. Our goal is to enable your agents to collaborate effectively on complex tasks, maximizing their collective intelligence and capabilities.

## Installation

Ensure you have Python >=3.10 <3.14 installed on your system. This project uses [UV](https://docs.astral.sh/uv/) for dependency management and package handling, offering a seamless setup and execution experience.

First, if you haven't already, install uv:

```bash
pip install uv
```

Next, navigate to your project directory and install the dependencies:

(Optional) Lock the dependencies and install them by using the CLI command:
```bash
crewai install
```
### Customizing

**Add your `OPENAI_API_KEY` into the `.env` file**

- Modify `src/research/config/agents.yaml` to define your agents
- Modify `src/research/config/tasks.yaml` to define your tasks
- Modify `src/research/crew.py` to add your own logic, tools and specific args
- Modify `src/research/main.py` to add custom inputs for your agents and tasks

## Running the Project

To kickstart your crew of AI agents and begin task execution, run this from the root folder of your project:

```bash
$ crewai run
```

This command initializes the research Crew, assembling the agents and assigning them tasks as defined in your configuration.

This example, unmodified, will run the create a `report.md` file with the output of a research on LLMs in the root folder.

## Understanding Your Crew

The research Crew is composed of multiple AI agents, each with unique roles, goals, and tools. These agents collaborate on a series of tasks, defined in `config/tasks.yaml`, leveraging their collective skills to achieve complex objectives. The `config/agents.yaml` file outlines the capabilities and configurations of each agent in your crew.

## Support

For support, questions, or feedback regarding the Research Crew or crewAI.
- Visit our [documentation](https://docs.crewai.com)
- Reach out to us through our [GitHub repository](https://github.com/joaomdmoura/crewai)
- [Join our Discord](https://discord.com/invite/X4JWnZnxPb)
- [Chat with our docs](https://chatg.pt/DWjSBZn)

Let's create wonders together with the power and simplicity of crewAI.
>>>>>>> 4264f56 (Initial commit: Research Crew AI project)
