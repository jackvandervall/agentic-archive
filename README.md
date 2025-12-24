# Agentic-Archive
This archive will consist of free agentic workflows in a plug-and-play format. Feel free to [reach out](#connect-with-me) for support or suggestions.


## Table of Contents
- N8N Agents
  - [Multi-Model Research Agent](https://github.com/jackvandervall/Agentic-Archive/blob/main/N8N%20Agents/Multi-Model%20Research%20Agent.json)
  - [RAG Agent](https://github.com/jackvandervall/Agentic-Archive/blob/main/N8N%20Agents/RAG%20Agent.json) (old)
  - [Data Analysis Agent](https://github.com/jackvandervall/Agentic-Archive/blob/main/N8N%20Agents/Data%20Analysis%20Agent.json)
  - [RAG and Research Agent](https://github.com/jackvandervall/Agentic-Archive/blob/main/N8N%20Agents/RAG%20and%20Research%20Agent.json) (new)
- N8N Tools
  - [Sonar Web Search Perplexity](https://github.com/jackvandervall/Agentic-Archive/blob/main/N8N%20Tools/Sonar%20Web%20Search%20(Perplexity%20API).json)
  - [Supabase Heartbeat Scheduler](https://github.com/jackvandervall/Agentic-Archive/blob/main/N8N%20Tools/supabase-heartbeat.json)


### Multi-Model Research Agent
The agent automates research by querying the Perplexity Sonar API using Claude and DeepSeek to gather, refine, and structure research findings. The Research Manager generates detailed insights from multiple queries, ensuring proper citations. The Research Compiler formats findings into structured Markdown with APA references. The Dataset Agent enhances results by sourcing extra datasets. Finally, all processed research is stored in a Supabase database for easy access and retrieval.

![Image](https://github.com/user-attachments/assets/91fceb3b-1658-41a2-aeaf-96733063e370)


### Retrieval-Augmented Generation(RAG) and Research Agent
A powerful RAG agent that will translate your natural language queries into actionable SQL queries to gain insights into any structured datasets. This agent is also able to execute the Multi-Model Research Agent in order to have a seamless integration of both dataset querying and research. 
1. **Natural Language to SQL** - The agent interprets user queries and generates structured SQL queries via RAG.
2. **Data Retrieval** - Fetches relevant structured data from databases (e.g., Supabase, PostgreSQL).
4. **Data Aggregation** - Supports SQL-based aggregation functions (e.g. MIN, MAX, AVG, SUM), filtering and grouping,
3. **Automated Chart Generation** - Converts results into JSON-based chart configurations.
4. **QuickChart Integration** - Renders visualizations dynamically.

![Image](https://github.com/user-attachments/assets/f6ef4652-6ee0-47c3-9163-44c8686e5450)


### Data Analysis Agent
An agent that automates data visualization by translating language queries into structured visualizations. Will provide an extensive range of visualizations when combined with a tool calling RAG agent. The agent generates introductory reports including visualizationsu using data provided by the RAG agent; it is then able to visualize various chart types (e.g., bar, scatter, line) with Quickchart to visualize trends dynamically.

![Image](https://github.com/user-attachments/assets/f6c184a6-e775-4689-99aa-933850337a60)


#### Example Query for Report and Visualization
"Create a report of the dataset including an introduction and multiple chart types."

- Generated an introduction to the dataset
- Key insights into leading salary designations
- Remote working distribution chart
- Line-chart of salary by experience level
- Employment status distribution

![Image](https://github.com/user-attachments/assets/b5c72cd4-1b97-47fe-a406-7f26e337710f)
See the full report here: https://imgur.com/a/rag-agent-data-analysis-example-from-basic-prompt-WVNuk78

### Web Search Tool (Perplexity Sonar / OpenRouter)
A tool that can be accessed by AI agents to perform web searches using the Perplexity Sonar API via HTTP requests, with [OpenRouter API](https://github.com/jackvandervall/Agentic-Archive/blob/main/N8N%20Tools/Sonar%20Web%20Search%20(OpenRouter%20API).json) support.

![Image](https://github.com/user-attachments/assets/45407c14-c77c-46f1-9362-4a60ac77c7d9)

### Supabase Heartbeat
A tool that can allows you to schedule poll requests to your Supabase database in order to keep it from being shut down after 7 days of inactivity. This can be used in contact page databases for example.

![Image](https://github.com/user-attachments/assets/ad0ee17c-623f-46e6-8ab4-68e965001353)


## Connect with Me
**LinkedIn:** [Jack van der Vall](https://www.linkedin.com/in/jackvandervall)  
**GitHub:** [jackvandervall](https://github.com/jackvandervall)  

