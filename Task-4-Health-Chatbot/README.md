Task 4: General Health Query Chatbot (Prompt Engineering with LLM)
Objective

To build a general health-related chatbot using a Large Language Model (Mistral API) with LangChain, focusing on prompt engineering, conversational memory, and safe response handling.

Tools & Technologies
Mistral API (LLM)
LangChain
Python
Chat Message Schema (System, Human, AI Messages)
Approach & Understanding

Instead of manually handling model prompts and responses, I used LangChain to structure the chatbot workflow. This made the system more modular and closer to real production-level LLM applications.

The key idea was to treat the conversation as a message-based system, where:

System Message defines the behavior of the chatbot
Human Message represents user input
AI Message stores model responses

This structure helps maintain context across the conversation instead of treating each query independently.

How the Chatbot Works
1. System Prompt Design

I defined a system-level instruction to control behavior:

The chatbot acts as a helpful health assistant
It provides general information only
It avoids diagnosis or unsafe medical advice
It keeps responses simple and user-friendly
2. LangChain Message Memory

I used LangChain’s message history structure to maintain context:

SystemMessage → defines rules and safety constraints
HumanMessage → user queries
AIMessage → chatbot responses

This allowed the chatbot to “remember” previous interactions within the session and respond in context instead of stateless replies.

3. Mistral API Integration

Instead of building separate logic for different models, I used Mistral through LangChain’s LLM interface. This allowed:

Unified interface for prompt handling
Easy switching of models without changing core logic
Cleaner and scalable architecture
4. Response Flow
User enters a health-related query
Message is added as HumanMessage
Conversation history is passed to the LLM
Mistral generates response based on full context
Response is stored as AIMessage
Updated memory is used for next interaction
Safety Handling

To ensure responsible AI usage:

The chatbot avoids medical diagnosis
It does not recommend unsafe treatments
It encourages consulting a professional for serious issues
Key Learning
Understood how LLM applications are structured using LangChain
Learned message-based memory systems (System / Human / AI)
Implemented prompt engineering for controlled responses
Gained experience integrating external LLM APIs (Mistral)
Understood how abstraction improves scalability in AI apps
Conclusion

This task helped me understand how modern AI chatbots are not just simple API calls, but structured systems using message memory, prompt control, and abstraction layers like LangChain to manage conversation flow efficiently.
