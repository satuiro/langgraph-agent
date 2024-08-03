# Langgraph Agent

## Problem Statement:

You have to perform the following operation using LLM with the help of function calling
Eg. `A+7=H, B+2=D, C-1=B.`
Using Langraph make an agentic model which will take query from user (i.e. add/subtract 5 steps to G)

## Installation and setup:

1. Clone the repository:

   ```sh
   git clone https://github.com/satuiro/langgraph-agent
   cd langgraph-agent
   ```

2. Create the conda environment and install necessary libraries:

   ```sh
   conda create -n agent python=3.12.4
   conda activate agent
   pip install langchain langchain-groq langgraph
   ```

3. Generate groq cloud API key from https://console.groq.com/keys and run the notebook agent.ipynb

## Using the code

The code can be run in the format of using queries as `queries = ['A+3','B-2','N+1','P+3', 'add 4, 2, 7 to A, B, G respectively']` and passing it down to the
agent in the entry mode that will call the ToolNode function accordingly.
