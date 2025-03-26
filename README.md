# Multi AI Agent System using CREW-AI

##### This Module implements working of Different agents for different tasks in sequential format using CREW-AI

**Implementation File:**  
📂 `./crew.py`
- Crew instance is responsible for managing the execution of tasks by a set of agents
  - **Further Breakdown:**
     1. **`Agents`** : Represents the list of agents responsible for completing tasks
     2. **`tasks`** : Represents the list of tasks assigned to the agents
     3. **`process`** : Specifies that tasks will be executed sequentially
    4. **`memory`** : Set to true to enable agents retain the previous context
    5. **`cache`** : Improves the memory management by providing the preious data/context stored in the memory
    6. **`max_rpm`** : Limits the rate of requests per minute to 100, preventing excessive API calls
    7. **`share_crew`** : Allows the Crew instance to be shared across different parts of the application


**Implementation File:**  
📂 `./agents.py`
- Responsible for defining different agents specifying role of the agent , the past story (backstory) of agent , expected behaviour(goal) and available tools. 

**Implementation File:**  
📂 `./tasks.py`
- Defined the tasks according to the user using CREW_AI `Task` class
