# LLM Agents MOOC - Fall 2024 - Lab Solutions

This repository contains my solutions for the lab assignments of the LLM Agents MOOC offered in Fall 2024.

## Lab 1: Summarizing Unstructured Data (Restaurant Reviews)

This lab focuses on using the AutoGen framework to process and analyze unstructured text data (restaurant reviews) to extract sentiment scores and aggregate them into an overall restaurant rating.

* **Objective:** Build a multi-agent system using AutoGen to fetch, analyze, and score restaurant reviews based on keywords indicating food quality and customer service.
* **Implementation:** Uses Python with the AutoGen framework and the GPT-4o-mini model.  The solution involves three agents: an entry point agent, a data fetching agent, and a review analysis agent.  The code is designed to handle different restaurant names and variations in review phrasing.
* **Files:**
    * `main.py`: Main implementation file.
    * `test.py`: Public test cases.
    * `calculate_overall_score`: Function to calculate the overall restaurant score.
    * `requirements.txt`: Project dependencies.
    * `restaurant-data.txt`:  Restaurant review data.

## Lab 2: LLM Security, Writing Attack Prompts

This lab focuses on crafting prompt injection attacks designed to extract a secret key embedded within the system message of an LLM.

* **Objective:** Write two attack prompts (`attack-1.txt` and `attack-2.txt`) to successfully extract a hidden alphanumeric secret key.
* **Methodology:**  Exploits prompt engineering techniques such as payload splitting, virtualization, and obfuscation.
* **Files:**
    * `attack-1.txt`: First attack prompt.
    * `attack-2.txt`: Second, more challenging attack prompt.
    * `student_info.json`: (Optional, for grading purposes)

## Lab 3: LLM Security, Writing Defense Prompts

This lab focuses on constructing a robust defense prompt to protect against prompt injection attacks.

* **Objective:** Create a defense prompt (`defense.txt`) that prevents the leakage of a secret key, even when faced with sophisticated attack prompts.
* **Methodology:** Employs various defense tactics, including clear instructions, adversarial prompt examples, and careful phrasing to guide the LLM's behavior.
* **Files:**
    * `defense.txt`: Defense prompt.
    * `student_info.json`: (Optional, for grading purposes)


## Getting Started

1. **Prerequisites:** Python 3.x, OpenAI API key (set as environment variable `OPENAI_API_KEY`).  Install required packages using `pip install -r requirements.txt`.
2. **Lab 1:** Run `python main.py` to interact with the restaurant review system. Run `python test.py` to check your solution against public test cases.
3. **Lab 2 & 3:** Create the `attack-1.txt`, `attack-2.txt`, and `defense.txt` files with your attack and defense prompts.  Test your prompts using the OpenAI playground.

