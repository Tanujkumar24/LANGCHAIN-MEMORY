
# Conversational AI: Memory Management and LangChain Applications

This repository demonstrates advanced memory management techniques and applications using LangChain for conversational AI systems. It includes a set of Jupyter notebooks that guide developers in creating efficient, scalable, and dynamic solutions for handling conversation context and memory.

---

## Table of Contents

1. [Project Overview](#project-overview)
2. [Key Features](#key-features)
3. [Technologies Used](#technologies-used)
4. [Setup and Installation](#setup-and-installation)
5. [Notebook Descriptions](#notebook-descriptions)
   - [Conversational_Summary_Memory.ipynb](#1-conversational_summary_memoryipynb)
   - [Langchain_memory_classes.ipynb](#2-langchain_memory_classesipynb)
   - [LCEL(Langchain_Expression_Language).ipynb](#3-lcellangchain_expression_languageipynb)
6. [How to Use](#how-to-use)
7. [Future Enhancements](#future-enhancements)
8. [Acknowledgments](#acknowledgments)
9. [License](#license)

---

## Project Overview

Conversational AI systems rely heavily on context management and memory efficiency to ensure meaningful, contextually relevant interactions. This repository explores:
- **Summary-Based Memory**: Condensing conversation histories to optimize memory usage.
- **Reusable Memory Classes**: Building modular and flexible memory structures.
- **Expression Language Integration**: Enhancing adaptability with LangChain Expression Language (LCEL).

Through hands-on examples in Jupyter notebooks, you’ll learn practical implementations for these features, enabling you to build robust conversational AI systems.

---

## Key Features

- **Dynamic Memory Management**: Optimize memory usage with tokenization and summarization techniques.
- **Reusable Classes**: Modular memory classes for long-term and short-term context management.
- **Expression Language**: Incorporate dynamic calculations and evaluations into conversations using LCEL.

---

## Technologies Used

- **Python 3.8+**: The primary programming language.
- **Jupyter Notebook**: Interactive environment for writing and testing code.
- **LangChain**: Framework for managing memory and workflows in AI-driven applications.
- **pip**: For dependency management.

---

## Setup and Installation

### Prerequisites

Ensure the following tools are installed:
- Python 3.8 or newer
- pip (Python package manager)
- Jupyter Notebook or Jupyter Lab

### Installation Steps

1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/conversational-ai-langchain.git
   cd conversational-ai-langchain
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Start Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

4. Open the desired notebook and run the code cells sequentially.

---

## Notebook Descriptions

### 1. Conversational_Summary_Memory.ipynb

This notebook introduces summary-based memory techniques to handle conversation context efficiently.

#### Highlights:
- Reduces memory overhead by summarizing conversation histories.
- Demonstrates integration with LangChain memory modules.

#### Code Example:
```python
from langchain.memory import SummaryMemory

memory = SummaryMemory()
memory.save_context({"input": "Hi, how are you?"}, {"response": "I'm fine, thank you."})
print(memory.load_memory_variables({}))
```

---

### 2. Langchain_memory_classes.ipynb

This notebook demonstrates how to create reusable and modular memory classes in LangChain.

#### Highlights:
- Implements conversation buffer memory for short-term and long-term context storage.
- Provides insights into storing and retrieving memory entries.

#### Code Example:
```python
from langchain.memory import ConversationBufferMemory

memory = ConversationBufferMemory()
memory.add_memory_entry("What is LangChain?")
print(memory.get_memory_entries())
```

---

### 3. LCEL(Langchain_Expression_Language).ipynb

This notebook focuses on integrating LangChain Expression Language (LCEL) to evaluate dynamic expressions.

#### Highlights:
- Enables logical calculations and dynamic adaptability in conversational systems.
- Demonstrates seamless integration into conversational workflows.

#### Code Example:
```python
from langchain.expression_language import evaluate_expression

result = evaluate_expression("2 + 2 * 5")
print("Result:", result)
```

---

## How to Use

1. Clone this repository to your local machine.
2. Install the required dependencies by running:
   ```bash
   pip install -r requirements.txt
   ```
3. Open the desired Jupyter notebook:
   ```bash
   jupyter notebook
   ```
4. Follow the comments and code examples in each notebook to learn and experiment with the concepts.

---

## Future Enhancements

- Expand support for additional memory modules in LangChain.
- Provide examples of integrating with external APIs and databases.
- Add a guide for deploying these solutions on cloud platforms.

---

## Acknowledgments

This repository was made possible thanks to:
- **LangChain Framework**: For providing a robust library to manage memory and workflows.
- **OpenAI Research**: For advancing the field of conversational AI.
- **Community Contributors**: For their valuable insights and shared tools.

---

## License

This project is licensed under the MIT License. Feel free to use, modify, and distribute the code as per the terms of the license.

---

## Contact

For queries, suggestions, or contributions, feel free to reach out:
- **Email**: tanuj.mangalapally@gmail.com
- **Portfolio**: [tanujkumar-portfolio](https://tanujkumar24.github.io/Tanujkumar-portfolio/)
