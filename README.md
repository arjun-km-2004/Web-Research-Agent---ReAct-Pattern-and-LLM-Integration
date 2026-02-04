# Web-Research-Agent---ReAct-Pattern-and-LLM-Integration
Approach
1. Planning: Using LLM for Research Question Generation
● The agent will use an LLM (for example: OpenAI's GPT or Gemini or Ollama for
local LLM) to assist in reasoning. The agent first asks the LLM to generate a list of
research questions related to the given topic.
● The LLM should suggest 5–6 well-structured questions that cover different
aspects of the topic.
● Example: If the topic is "Climate Change," the LLM may generate questions like:
○ What are the main causes of climate change?
○ How has global temperature changed over the past century?
○ What policies are in place to combat climate change?
2. Acting: Web Search for Gathering Information
● The agent will take each research question and search the web to find relevant
and recent information.
● The agent should extract key points from search results and store them.
3. Report Generation
● After collecting data for all questions, the agent will compile a structured report
summarizing its findings.
● The report should have a title, an introduction, sections for each research
question, and a conclusion.
Architecture
Design Patterns Used
To build a scalable and well-structured agent, we will use:
1. Planning Pattern – The agent plans its research steps (generating questions
before searching).
2. Tool-Use Pattern – The agent selects and uses tools (LLM and web search) to
achieve its goal.
Steps to Complete the Assignment
1. Set Up the LLM:
○ Use an LLM API (such as Groq API or Gemini API) or local LLM using Ollama
to assist in reasoning. Make sure to set up an API key and install any
required libraries like OpenAI in Python.
2. Implement the Agent Class
● Define an Agent class that:
○ Takes a topic as input.
○ Uses an LLM to generate research questions.
○ Searches the web for answers.
○ Stores and structures the collected information.
2. Use LLM for Planning
● Implement a function that queries an LLM to generate relevant research questions.
3. Use Web Search for Acting
● Implement a function that performs a web search for each question and extracts
relevant information such as title and content of different search results
● Use the Tavily library in Python and extract the title and content of every search
result.
4. Compile the Final Report
● Format the collected data into a structured report
Expected Deliverables
1. Code Submission
○ A Python script or ipynb file implementing the ReAct agent using LLM and a
web search tool.
2. Report
i. A brief explanation (in markdowns) describing how you used the LLM
for reasoning. Explain how the reasoning step works.
ii. Explain code and flow of your program.
