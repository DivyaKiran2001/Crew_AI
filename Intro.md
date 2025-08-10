### What is Crew AI ?

CrewAI is a framework that allows us to create AI agents where each agent has its own
expertise and instructions.Together, the agent will work towards solving one large 
complex problems.

CrewAI is a lean, lightning-fast Python framework built entirely from scratch—completely independent of LangChain or other agent frameworks.

**Examples :**

1. Stock Analysis
2. Trip Planner
3. Game Builder

### How CrewAI Works 

**1. Agents**

**Properties :**

**Role:** The agent’s function (e.g., Researcher, Writer, Editor)

**Goal:** Their overarching objective guiding behavior

**Backstory**: Contextual background for more nuanced responses

**Additional attributes:** **Tools, memory settings, LLM configuration, execution constraints,** etc.


**2. Tools :** There are two types of tools

- Built in tools
- Custom tools (custom python definitions)

**3. Task :** Tasks are jobs that agents need to Complete

Task in CrewAI can be designed to require collaboration between agents.
**Ex:** One agent might gather data while another analyzes it

| Property             | Description                                                                        |
| -------------------- | ---------------------------------------------------------------------------------- |
| **description**      | Clear, detailed instructions for the task — tells the agent exactly what to do.    |
| **agent**            | The specific **Agent** assigned to perform this task.                              |
| **expected\_output** | A description of what the final result should look like (format, quality, etc.).   |
| **context**          | Optional additional info or results from previous tasks that this task depends on. |
| **tools**            | (Optional) Specific tools the task can use — could be LangChain tools, APIs, etc.  |
| **async\_execution** | Whether the task runs asynchronously (in parallel with others).                    |
| **retry\_count**     | How many times the task should retry if it fails.                                  |
| **callback**         | A function to run after the task finishes (can be used to post-process results).   |

**4. Process :**

In CrewAI, a Process is the big picture — it’s the workflow that coordinates multiple agents and tasks to work together toward a common goal.

If a Task is like a single to-do item, a Process is the entire project plan.

It decides what order tasks happen in.

It manages dependencies between tasks.

It controls how agents collaborate.





















