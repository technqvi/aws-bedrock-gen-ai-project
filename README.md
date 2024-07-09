# Amazone Bedrock GenAI LLM Project
Implement Generative AI Project   such as Knowledge Base, Agent Base, Text Classification, Text Generation, Data/Document Extraction  on  AWS Platform : Amazon Bedrock, Langchain, Claude.ai ,llamaindex.ai , Vector Database (Pinecone,Open Search  Serverless, PGVector)

## Incident Knownledge Base
<img src="images/incident-kb.png">

* Amazon Bedrock streamlines IT incident management by ingesting incident data, transforming user queries into embeddings, searching for relevant context in a VectorDB, and generating accurate responses using a reference model. 
* This workflow enables the IT-Incident KB Chatbot to provide efficient and contextually relevant answers to user questions which are historical incident cases  in order to streamline  the overall incident management process to fix any incident issues for customer efficiently.

## Incident Agent
<img src="images/incident-agent.png"/>
The image illustrates the process of the Incident-Agent to orchestrate various tasks for IT Incident Manangement System including

* Retrieving Historical incident data from the knowledge base is retrieved to assist in resolving the incident.
* Fetching real-time incident data in order to updating the status, and adding incident details to the Agent toward the AWS Lambda function to database right away. 


## Document Extraction to Structure Data For Analystics.
<img src="images/data-extraction.jpg">

It involved a process that uses a Large Language Model (LLM) Generative AI model to extract data from resumes in PDF format. Here's a breakdown of the process in bullet points:

* The process starts with unstructured data in PDF format being ingested. This could include resumes in various formats and styles.
* The LLM Generative AI model then extracts data from the PDF files.
* The extracted data is then stored in a structured format, like a JSON file. This allows for easier organization and analysis of the information.
* It's important to note that, It can be used to various kind of document such as resume, invoice billing, preventive maintenance document with varying layouts/pattern

## Incident Severity Level Classification (Comming Soon)
<img src="images/incident-severity-classification.jpg">

The image depicts a process for identifying severity level to respond to IT incidents. Here are the steps in the flowchart, broken down into bullet points:

* The process starts with an IT incident being opened. There are two options at this point:
* If Model classified as critical or major incident, then an alert 
* The possible severity levels are Critical ,Major ,Minor, Cosmetic
* Depending on the severity level of the incident, different actions are taken.

## Incident Query & Reporting  By Natural Language to SQL Query Converter (Comming Soon)
<image src="images/incidnet_text_to_sql.png">
The image illustrates a process flow for a user to query data from a database using natural language. Here's a step-by-step description:

1. The user inputs a query in natural language format.

2. The natural language query is sent to an Amazon Bedrock service, which is represented by an icon showing a brain with a question mark.

3. The Amazon Bedrock service processes the natural language query and passes it to an AWS Lambda function, represented by the Lambda icon.

4. The AWS Lambda function converts the natural language query into a SQL query.

5. The generated SQL query is then used to retrieve data from an AWS Glue Data Catalog, which is connected to an Amazon Athena service and an Amazon RDS (Relational Database Service) database.

6. The Athena service and RDS database execute the SQL query and fetch the requested data.

7. The query result is returned, and an example of the result data is shown in a CSV (Comma-Separated Values) format at the bottom of the image.

This process demonstrates how a user can interact with a database using natural language queries, which are transformed into SQL queries behind the scenes to retrieve the desired data from the connected data sources.
 
