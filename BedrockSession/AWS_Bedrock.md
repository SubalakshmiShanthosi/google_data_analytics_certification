# Amazon Bedrock

Introduction to Bedrock
   Key features
   Demo RAG, agents and guardrails

AWS Skillbuilder
    Free badges on GenAI and Bedrock
    Game based learning
    Earn badges

Impact of Generative AI

    History - tracing back - Eliza (1978) - chatbot - rule based learning
    Ethical computing (Eliza - 1982) -> Good bad- responsible use. 
    1986 - AI - Control systems on nuclear reactors - AI usecase

About 75% of the value the gen ai usecases could deliver falls on four category - software engineering, research and development, customer operations, marketing and sales.

By 2026 - 80% of genAI appln adoption on enterprises on production scale

79% respondents - say genAI will be within various business functions

Risk and challenges with GenAI applications

    Providing incorrect answers (hallucinations) - Mitigation - Implementing Bedrock Guardrails
    Leaking confidential information - Mitigation - Implementing Bedrock Guardrails
    Insufficient or outdated data
    Accessing multiple FM's and new versions
    Lacking understanding of your business and customers.
    Risk of copyright violations --- Pretty challenging ---  Work can be stolen -- trade secrets can be reveiled while retraining FM.

Building model from scratch -- Heavy, would take more time.

Understand the business problem
    Algo to solve - go rule based solving
    Off the self AI package - Use that
    ML - Learning from patterns and predict for future

Choice -- models to choose, model evaluation

Responsible AI - Data privacy and security.
AWS Guardrails

Customization - Prompt Engineering, Bedrock RAG, Agentic AI

Generative AI = The overall technology that creates new content (text, images, etc.). LLMs = A specific type of Generative AI that focuses on text. Amazon Bedrock = A service that lets businesses easily use powerful AI models without building them from scratch

Question? - Any ability to check on cost of GenAI interface for a usecase - Amazon Bedrock pricing - pay as you go - ondemand and batch, vision throughput

Single API - access to large variety of FMs.

Agent AI - Amazon Bedrock - Learn more on Agent Memory - Number of sessions to hold -(it's implication to cost)

RAG  - is better - large data huge data drift at hour/ day level

Model level or agent level guardrails -- Look into bedrock guardrails (creation, attaching to agent - about knowledge base and limitations to restrict the chat response)

Also on guardrails - No PII/ Harmful category to block and harmful categories. Protect from prompt attacks too..

Guardrails - Regex based masking or blocking of data on response ---
Any ways to test the regex?

TODO => Agent - Chain of thought trace and ability to understand the guardrails action while giving response.

Look for agentic ai invocation - eventdriven, trigger function

Agent - Action group
