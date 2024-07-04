# Amazone Bedrock GenAI LLM Project
## Incident Knownledge Base
<img src="images/incident-kb.png">
* Amazon Bedrock streamlines IT incident management by ingesting incident data, transforming user queries into embeddings, searching for relevant context in a VectorDB, and generating accurate responses using a reference model. 
* This workflow enables the IT-Incident KB Chatbot to provide efficient and contextually relevant answers to user questions which are historical incident cases  in order to streamline  the overall incident management process to fix any incident issues for customer efficiently.

## Incident Agent
<img src="images/incident-agent.png"/>
The image illustrates the incident management workflow using the Amazon Bedrock knowledge base. The process involves the Incident-Agent receiving real-time incident data, updating the status, and providing details to the Agent.
* The Agent performs actions, updates incident details, and adds them to the AWS Lambda bot actions. 
* Historical incident data from the knowledge base is retrieved to assist in resolving the incident.

### Incident Severity Level Classification
<img src="images/jpg-incident-severity-classification.jpg">

The image depicts a process for identifying severity level to respond to IT incidents. Here are the steps in the flowchart, broken down into bullet points:

* The process starts with an IT incident being opened. There are two options at this point:
* If Model classified as critical or major incident, then an alert 
* The possible severity levels are Critical ,Major ,Minor, Cosmetic
* Depending on the severity level of the incident, different actions are taken.
 
### Data Extraction from Unstructure to Structure.
<img src="images/jpg-data-extraction.jpg">

It involved a process that uses a Large Language Model (LLM) Generative AI model to extract data from resumes in PDF format. Here's a breakdown of the process in bullet points:

* The process starts with unstructured data in PDF format being ingested. This could include resumes in various formats and styles.
* The LLM Generative AI model then extracts data from the PDF files.
* The extracted data is then stored in a structured format, like a JSON file. This allows for easier organization and analysis of the information.
* It's important to note that, It can be used to various kind of document such as resume, invoice billing, preventive maintenance document with widely varying layouts/pattern