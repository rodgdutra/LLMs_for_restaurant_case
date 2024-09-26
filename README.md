# Leveraging LLMs for Restaurant Solutions: A Case of Study

## Introduction

In the rapidly evolving landscape of artificial intelligence, Large Language Models (LLMs) have emerged as powerful tools for enhancing various sectors, including the restaurant industry. This project focuses on leveraging LLMs to provide innovative solutions tailored specifically for restaurants, using the mock-up case study of "Burger Bliss" a fictional restaurant featuring a mock up menu. By harnessing the capabilities of LLMs, we aim to streamline restaurant operations, improve customer interactions, and enhance overall service delivery.

The Burger Bliss menu serves as our primary data source, enabling us to explore various applications of LLMs in a restaurant context. We will demonstrate how LLMs can be utilized to respond to customer inquiries, provide menu information, and facilitate a more engaging dining experience through natural language interactions.

## Project Overview

In this project, we will explore different methodologies for utilizing the Burger Bliss menu with LLMs:

### 1. [**Retrieval-Augmented Generation (RAG) Workflow**](https://github.com/rodgdutra/LLMs_for_restaurant_case/blob/main/restaurant_rag.ipynb): 
here we implemented a RAG workflow that allows for enhanced query responses based on relevant menu items. This approach combines information retrieval with language generation, ensuring that our LLM provides accurate and contextually relevant answers to customer inquiries.

Some cool results:

Before the RAG process:
```
Input text: Do you have any vegetarian burger option in the menu?

Output text:
I am unable to access real-time information, therefore I cannot provide a menu at this time. For the most up-to-date options and descriptions of the hamburgers offered, please check the menu on the restaurant's website or social media pages.
```

After the RaG process:
```
Query: Do you have any vegetarian burger option in the menu?
[INFO] Time taken to get scores on 6 embeddings: 0.00012 seconds.
Answer:

Sure, the relevant passage from the context is:  - 5: Avocado Veggie Burger -
$10.49 A flavorful black bean and quinoa patty topped with creamy avocado, fresh
spinach, and tangy ranch dressing on a multigrain bun. Healthy never tasted so
good!

Therefore, the answer to the query is: Absolutely! We have our Avocado
Veggie Burger, which is made with a black bean and quinoa patty. Would you like
to try that?
```

### 2. [**Fine-Tuning Processes**](https://github.com/rodgdutra/LLMs_for_restaurant_case/blob/main/restaurant_finetune.ipynb):
In addition to the RAG workflow, here we explored fine-tuning techniques such as Low-Rank Adaptation (LoRA). By applying these techniques, we can customize the LLM to better understand and respond to specific queries related to the Burger Bliss menu, ensuring that the generated responses are not only informative but also tailored to the unique offerings of the restaurant.

Through this case study, we aim to illustrate the potential of LLMs in revolutionizing the restaurant industry and providing enhanced solutions that meet the needs of both restaurant operators and their customers.

**TODO**: In the near future, we will integrate the RAG process with the fine-tuning approach, aiming to harness the strengths of both methods. This combination will allow us to create a close representation of a real-world use case, where every customer order matters. Through this integration, we can enhance the model's performance and ensure it delivers accurate and relevant information in a dynamic restaurant environment.
