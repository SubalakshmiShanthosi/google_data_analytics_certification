# Episode 4: Implementing Knowledge Bases - Deep Dive with AWS! Amazon Bedrock - AI Agents

RAG - Never let the base model give response from it's training data - Always have it infer after using context from Knowledge base to reduce hallucinations/ incorrect interpretation.

Example - Giving customer incorrect information solely relying on FM data (it's last training data of FM is few years before) => Knowledge base with recent data. 

When do I need an Knowledge base/ When do I call a tool?

RAG Components?
    Key component in GenAI appln
    Gathering custom database
    Put the data to vector database
    User creates the prompt
    Augment the prompt from user with data from vector store --> Adding context to the prompt and then call the LLM chatbot for answering

    RAG - Four step process - Create the knowledge base - FAQ (Embeddings database with internal databases - text or multi modal (image/visuals))

    Orchestrator that takes user query and then look for the vector store to see any similar questions + prev response 

    Retreiver - Fetches relevant context from vector database and ranks the response

How Knowledge bases work?
    Phases of Knowledge bases - Two phases - Preprocessing
        From data store - Splitting into chunks
        Generating embeddings --
    Creating with structured data store / Knowledge base with Kendra 

    Vector store - Amazon Neptune, Opensearch Serverless

    Datasources - Web crawler  - It obeys the rule of internet (comply based on robots.txt) - Crawl only if the webpage is indexed (9 diff URL max per knowledge base)

Evaluating knowledge base
     IAM role with appropriate permissions S3 bucket, bedrock 
     CORS on S3 setting
     Score based on what kind of responses the Bedrock will give for the user prompt based on the data on S3 data storage.


    JSONL - Prompt question, and the ground truth
     Metrics - 10 different - Citation precision, correctnes, completeness,, Helpfullness, faithfulness, stereotyping (much more.)
