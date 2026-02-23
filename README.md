# Autonomous-Software-Engineering-Sprint-Assistant
This is an Agentic Sprint Assistant that takes a product feature request and autonomously understands it, breaks it into tasks, assigns roles, generates code, writes tests, reviews its own output and evaluates quality. This simulates a real Agile sprint cycle using AI agents.

# Project Architecture
```mermaid
flowchart TD;
        A(["User Input"])
        A --> |Feature Request| B["Defining LLM For Generating Text"]
        B --> C{"Defining Agents"}
        C --> D["Product Manager"]
        C --> E["Architect"]
        C --> F["Developer"]
        C --> G["Tester"]
        C --> H["Reviewer"]
        D --> |Managed By| I["Langraph Orchestrator"]
        E --> I["Langraph Orchestrator"]
        F --> I["Langraph Orchestrator"]
        G --> I["Langraph Orchestrator"]
        H --> I["Langraph Orchestrator"]
        I --> J["Agents Evaluation"]
        J --> K["Final Sprint Report"]
```

