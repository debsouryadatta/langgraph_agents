
### Project-1 Overview:
In this project, we'll demonstrate the power of LangGraph by building a multi-step text analysis pipeline. Our use case will focus on processing a given text through three key stages:

- Text Classification: We'll categorize the input text into predefined categories (e.g., News, Blog, Research, or Other).
- Entity Extraction: We'll identify and extract key entities such as persons, organizations, and locations from the text.
- Text Summarization: Finally, we'll generate a concise summary of the input text.


### Steps:
1. `poetry new langgraph`, `poetry env use python3.11`, `poetry shell`, `poetry add langchain langchain_core langchain_community langgraph`
2. Building the text processing pipeline
    - Define State & Initialize LLM
    - Define Node Functions
    - Create tools & Build Workflow
    - Visualize the Workflow
    - Testing the Pipeline

3. `poetry add langchain_groq`, `poetry add ipython`, `poetry add dotenv`
4. `poetry run langgraph_stuff/proj_1.py`
```js
const data = { 
    
    'text': '\nOpenAI has announced the GPT-4 model, which is a large multimodal model that exhibits human-level performance on various professional benchmarks. It is developed to improve the alignment and safety of AI systems.\nadditionally, the model is designed to be more efficient and scalable than its predecessor, GPT-3. The GPT-4 model is expected to be released in the coming months and will be available to the public for research and development purposes.\n', 
    
    'classification': "Category: News\n\nReason: The text appears to be a factual report about a recent development in the field of AI, specifically the announcement of the GPT-4 model by OpenAI. The language used is formal and objective, and the text provides information about the model's features and expected release date, which is typical of news articles.", 
    
    'entities': ['OpenAI', 'GPT-4', 'GPT-3'], 
    
    'summary': 'OpenAI has announced the GPT-4 model, a large multimodal model that exhibits human-level performance and is designed to be more efficient and safer than its predecessor.' 

}
```

---


### Project-2 Overview:
Project Overview: Essay Grading System
In this tutorial, we'll demonstrate the power of LangGraph by building a multi-step essay grading system. Our use case will focus on processing a given essay through four key stages:

- Content Relevance: Assesses how well the essay addresses the given topic
- Grammar Check: Evaluates the essay's language usage and grammatical correctness
- Structure Analysis: Examines the organization and flow of ideas in the essay
- Depth of Analysis: Gauges the level of critical thinking and insight presented

### Steps:
1. Building The Essay Grading System pipeline
    - Define State & Initialize LLM
    - Define Node Functions
    - Create tools & Build Workflow
    - Visualize the Workflow
    - Essay Grading Function
    - Testing the Pipeline
2. `poetry run langgraph_stuff/proj_2.py`
```
Final Essay Score: 0.88

Relevance Score: 1.00

Grammar Score: 0.95

Structure Score: 0.90

Depth Score: 0.70
```

---

