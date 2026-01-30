# Agentic-Archive

> **Note:** This repository is preserved as a technical showcase for educational purposes. It represents the "hard-coded" era of agentic engineering (Early 2025).

## Description
This repository contains a collection of agentic workflows built in early 2025 for data analysis and research purposes.

**Context:**
At the time of development, standard agentic interfaces (like MCP or native Sandboxed Code Interpretation) did not exist or were not widely accessible. To achieve autonomous behavior, logic had to be explicitly built into rigid pipelines:

* **Web Search:** via Perplexity Sonar API.
* **Deep Research:** Multi-model orchestration.
* **Data Visualization:** JSON-to-Visual generation.

Please note that some of these methods may now be superseded by modern, native "Deep Research" agents, MCP, or coding tools released since 2025. They are preserved here for reference and educational purposes.

## Table of Contents
- Agentic
  - [Multi-Model Research Agent](https://github.com/jackvandervall/Agentic-Archive/blob/main/N8N%20Agents/Multi-Model%20Research%20Agent.json)
  - [Data Analysis Agent](https://github.com/jackvandervall/Agentic-Archive/blob/main/N8N%20Agents/Data%20Analysis%20Agent.json)
  - [RAG and Research Agent](https://github.com/jackvandervall/Agentic-Archive/blob/main/N8N%20Agents/RAG%20and%20Research%20Agent.json)
- Tooling
  - [Sonar Web Search Perplexity](https://github.com/jackvandervall/Agentic-Archive/blob/main/N8N%20Tools/Sonar%20Web%20Search%20(Perplexity%20API).json)
  - [Supabase Heartbeat Scheduler](https://github.com/jackvandervall/Agentic-Archive/blob/main/N8N%20Tools/supabase-heartbeat.json)


### Multi-Model Research Agent
The agent automates research by querying the Perplexity Sonar API using Claude and DeepSeek to gather, refine, and structure research findings. The Research Manager generates detailed insights from multiple queries, ensuring proper citations. The Research Compiler formats findings into structured Markdown with APA references. The Dataset Agent enhances results by sourcing extra datasets. Finally, all processed research is stored in a Supabase database for easy access and retrieval.

> **Note:** Modern reasoning models (e.g., o3, Deep Research) now handle this loop internally without explicit orchestration nodes.

![Image](https://github.com/user-attachments/assets/91fceb3b-1658-41a2-aeaf-96733063e370)


### Retrieval-Augmented Generation (RAG) and Research Agent
A RAG agent that translates natural language queries into actionable SQL queries to gain insights into structured datasets. This agent also executes the Multi-Model Research Agent to seamlessly integrate dataset querying with qualitative research.
1. **Natural Language to SQL** - The agent interprets user queries and generates structured SQL queries via RAG.
2. **Data Retrieval** - Fetches relevant structured data from databases (e.g., Supabase, PostgreSQL).
3. **Data Aggregation** - Supports SQL-based aggregation functions (e.g. MIN, MAX, AVG, SUM), filtering, and grouping.
4. **Automated Chart Generation** - Converts results into JSON-based chart configurations.
5. **QuickChart Integration** - Renders visualizations dynamically.

> **Note:** This approach is brittle compared to modern database MCPs, which expose the actual schema directly to the LLM for deterministic querying, as opposed to hardcoding the schema into the context.

![Image](https://github.com/user-attachments/assets/f6ef4652-6ee0-47c3-9163-44c8686e5450)

### Data Analysis Agent
An agent that automates data visualization by translating language queries into structured visualizations. It generates introductory reports including visualizations using data provided by the RAG agent. It visualizes various chart types (e.g., bar, scatter, line) via QuickChart to identify trends dynamically.

"Create a report of the `data_science_salaries.csv` dataset including an introduction and diverse visualizations."

- Generated an introduction to the dataset
- Key insights into leading salary designations
- Remote working distribution chart
- Line-chart of salary by experience level
- Employment status distribution

> **Note:** This method is rigid; if the generated JSON format was slightly off, the chart failed. Modern agents simply write and execute Python/React code to render interactive charts instantly.

![Image](https://github.com/user-attachments/assets/f6c184a6-e775-4689-99aa-933850337a60)

### Web Search Tool
A tool accessed by AI agents to perform web searches using the Perplexity Sonar API via HTTP requests, with [OpenRouter API](https://github.com/jackvandervall/Agentic-Archive/blob/main/N8N%20Tools/Sonar%20Web%20Search%20(OpenRouter%20API).json) support.

> **Note:** This is a manual API Wrapper using standard HTTP Requests to allow agents to read web pages via Perplexity Sonar.

![Image](https://github.com/user-attachments/assets/45407c14-c77c-46f1-9362-4a60ac77c7d9)

### Supabase Heartbeat
A tool that allows you to schedule poll requests to your Supabase database to prevent it from pausing after 7 days of inactivity. Useful for hobby-tier projects.

![Image](https://github.com/user-attachments/assets/ad0ee17c-623f-46e6-8ab4-68e965001353)

## Credits

Jack van der Vall

## License

This project is licensed under the MIT License.
