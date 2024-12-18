# Conversational AI: Memory Management and LangChain Applications

This repository contains a series of Jupyter notebooks that showcase advanced techniques in conversational AI, including memory management, the implementation of LangChain memory classes, and the use of LangChain Expression Language (LCEL). Each notebook is designed to provide practical insights and hands-on examples to build scalable and efficient conversational systems.

---

## Table of Contents

1. [Project Overview](#project-overview)
2. [Key Features](#key-features)
3. [Setup and Installation](#setup-and-installation)
4. [Notebook Explanations](#notebook-explanations)
   - [Conversational_Summary_Memory.ipynb](#1-conversational_summary_memoryipynb)
   - [Langchain_memory_classes.ipynb](#2-langchain_memory_classesipynb)
   - [LCEL(Langchain_Expression_Language).ipynb](#3-lcellangchain_expression_languageipynb)
5. [How to Run](#how-to-run)
6. [Acknowledgments](#acknowledgments)
7. [License](#license)

---

## Project Overview

The goal of this project is to explore and implement memory management solutions for conversational AI systems using LangChain. The notebooks cover:
- Summarizing long conversations to reduce memory usage.
- Creating reusable and efficient memory classes for context management.
- Implementing LCEL for dynamic and adaptive conversational AI workflows.

By following the examples in this repository, developers can learn to design and deploy robust memory systems for their AI applications.

---

## Key Features

- **Summary-Based Memory**: Learn to compress conversation histories into summaries to save computational resources.
- **LangChain Memory Classes**: Implement modular memory solutions for conversational systems.
- **Dynamic Expression Language**: Utilize LangChain Expression Language (LCEL) for enhanced AI adaptability.

---

## Setup and Installation

### Prerequisites

Make sure the following are installed on your system:
- Python 3.8 or higher
- Jupyter Notebook or Jupyter Lab
- pip for package installation

### Installation Steps

1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/conversational-ai-langchain.git
   cd conversational-ai-langchain

### Notebook Explanations
1. Conversational_Summary_Memory.ipynb
This notebook demonstrates how to create summary-based memory for conversational AI systems.

Key Highlights:
Purpose: Reduce memory overhead by summarizing conversation histories dynamically.
Techniques:
Tokenization and text summarization.
Integration with LangChain's memory modules.
Code Example:
python
Copy code
from langchain.memory import SummaryMemory

memory = SummaryMemory()
memory.save_context({"input": "Hi, how are you?"}, {"response": "I'm fine, thank you."})
print(memory.load_memory_variables({}))
2. Langchain_memory_classes.ipynb
This notebook introduces the concept of memory classes in LangChain, demonstrating how to handle conversation context effectively.

Key Highlights:
Purpose: Develop reusable memory classes for AI systems.
Concepts:
Storing and retrieving memory entries.
Managing long-term and short-term memory.
Code Example:
python
Copy code
from langchain.memory import ConversationBufferMemory

memory = ConversationBufferMemory()
memory.add_memory_entry("What is LangChain?")
print(memory.get_memory_entries())
3. LCEL(Langchain_Expression_Language).ipynb
This notebook covers the LangChain Expression Language (LCEL) and its use cases in building dynamic conversational AI solutions.

Key Highlights:
Purpose: Enable AI models to process and evaluate dynamic expressions.
Features:
Evaluate logical expressions.
Integrate LCEL into larger AI workflows.
Code Example:
python
Copy code
from langchain.expression_language import evaluate_expression

result = evaluate_expression("2 + 2 * 5")
print("Result:", result)
How to Run
To run the notebooks:

Start Jupyter Notebook:
bash
Copy code
jupyter notebook
Open the desired notebook, e.g., Conversational_Summary_Memory.ipynb.
Execute the cells sequentially to see the implementation.
For example:

bash
Copy code
jupyter notebook Conversational_Summary_Memory.ipynb
Acknowledgments
This repository was made possible thanks to:

LangChain Framework: A robust library for building AI-driven pipelines.
OpenAI Research: For advancing conversational AI technologies.
Community Contributors: For sharing insights and tools.
License
This project is licensed under the MIT License. For more information, refer to the LICENSE file in the repository.
