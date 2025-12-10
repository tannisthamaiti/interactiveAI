## Month 1: The Physics of LLMs & Prompting Fundamentals
Goal: Understand how models "think" and master manual control over their outputs.

Week 1: LLM Architecture Basics

How Transformers work (simplified): Tokens, Context Windows, and Attention Mechanisms.

The difference between Base Models (e.g., Llama 3 Base) vs. Instruct/Chat Models (e.g., GPT-4o, Claude 3.5 Sonnet).

### Key Concept: Probabilistic generation vs. deterministic code.
Week 2: Core Prompting Techniques

Zero-shot vs. Few-shot prompting (providing examples).

Role-playing (Persona pattern): "Act as a Senior Python Engineer..."

Delimiters and XML tagging: Structuring inputs to prevent model confusion.

### Week 3: Advanced Reasoning Structures

Chain-of-Thought (CoT): Forcing the model to "show its work" to improve logic.

Tree-of-Thought & Self-Consistency: Generating multiple paths and picking the best one.

Project: Build a "Logic Puzzle Solver" using CoT techniques.

### Week 4: The System Prompt

Designing robust System Instructions to govern behavior.

Output Formatting: Forcing JSON, Markdown, or SQL outputs for programmatic use.

## Month 2: Automated Prompting & Evaluation
Goal: Stop guessing if a prompt is good and start measuring it.
## Week 5: Iterative Prompt Development
The "Prompt Cycle": Write $\rightarrow$ Test $\rightarrow$ Refine.

Using LLMs to write prompts (Meta-prompting).

### Week 6: Prompt Evaluation (Evals)
How to score subjective text? (Answer: Use a stronger LLM as a judge).
Building a "Golden Dataset" of correct answers to test against.

### Week 7: Prompt Engineering for Developers (API)
Moving from ChatGPT web UI to OpenAI/Anthropic APIs.
Parameters: Temperature, Top_P, Frequency Penalty.

### Week 8: LLM Security & Safety
Prompt Injection attacks (jailbreaking).
Defensive Prompting: Guardrails and sanitization.
Project: "Jailbreak the Bot" challenge (secure your bot against class attacks).

## Month 3: Building Applications (LangChain/LlamaIndex)
Goal: Connect the LLM to logic and workflows.
### Week 9: Introduction to Orchestration Frameworks
Why do we need LangChain or LlamaIndex?
Chains: Linking multiple prompts together (Input $\rightarrow$ Prompt A $\rightarrow$ Prompt B $\rightarrow$ Output).
### Week 10: Memory Management
Handling context limits: Buffer Memory, Summary Memory, and Window Memory.
How to maintain a conversation history in an API app.
### Week 11: Structured Output Parsing
Using Pydantic/Zod to guarantee the LLM returns valid code/JSON.
Error handling: What to do when the LLM hallucinates a format.
### Week 12: Application Architecture
Latencies and cost management (Token counting).
Project: Build a "YouTube Video Summarizer" (Input URL $\rightarrow$ Transcript $\rightarrow$ Summary).

## Month 4: Retrieval Augmented Generation (RAG)
Goal: Connect the LLM to your own private data (PDFs, Company Docs).
### Week 13: Embeddings & Vector Databases
What are Embeddings? (Converting text to numbers).
Intro to Vector DBs: Pinecone, Weaviate, or ChromaDB.
### Week 14: RAG Pipeline Construction
Ingestion: Chunking strategies (splitting text effectively).
Retrieval: Semantic search vs. Keyword search.
Synthesis: Feeding retrieved chunks into the LLM context.
### Week 15: Advanced RAG
Hybrid Search (combining keywords + semantics).
Reranking: Re-sorting search results for better relevance.
### Week 16: RAG Evaluation
RAGas framework: Measuring "Faithfulness" and "Answer Relevance."
Project: "Chat with your PDF" application.

## Month 5: Agents & Tool Use
Goal: Give the LLM "hands" to perform actions (Search web, run code, query DB).
### Week 17: Function Calling (Tool Use)
Defining functions for the LLM (e.g., get_weather(city)).
The ReAct Pattern: Reasoning + Acting loop.
### Week 18: Building Autonomous Agents
Single-agent patterns vs. Multi-agent collaboration.
Using tools: Web browsing, Calculator, Python REPL.
### Week 19: Agentic Frameworks
Deep dive into LangGraph or CrewAI.
Managing agent loops and preventing infinite loops.
### Week 20: Fine-Tuning (Intro)
When to prompt vs. when to fine-tune.
PEFT (Parameter-Efficient Fine-Tuning) and LoRA high-level overview.
Project: A "Travel Agent" that can search flights, check weather, and book a generic itinerary.
