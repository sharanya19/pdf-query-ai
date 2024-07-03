# PDF Query AI

PDF Query AI integrates LangChain4j's capabilities to ingest PDF documents, process them into embeddings using specific AI models, and provide conversational query responses based on the ingested content. This project demonstrates a practical application of AI in document querying scenarios.

## Features
- Ingests PDF documents into a Cassandra database via LangChain4j.
- Utilizes OpenAI's chat model for generating responses to queries.
- Provides a RESTful API endpoint for querying PDF documents.

## Technologies Used
- Java 21
- Spring Boot 3.3.1
- LangChain4j 0.25.0
- OpenAI API
- Apache PDFBox

## Setup Instructions

### Prerequisites
- Java Development Kit (JDK) 21 or higher
- Maven 3.6.3 or higher
- AstraDB credentials (token, database ID, and region)

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/pdf-query-ai.git

2. Navigate to the project directory:

   ```bash

    cd pdf-query-ai
   

3. Update the AstraDB credentials in PdfAssistanceConfig.java:

- String astraToken = "YOUR_ASTRA_DB_TOKEN";
- String databaseId = "YOUR_DATABASE_ID";

4. Build
- Build the project using Maven:
  ```bash

    mvn clean install
  
5. Running the Application
- Run the application using Maven:

  ```bash

  mvn spring-boot:run
- The application will start at http://localhost:8080.


### API Endpoint

- Endpoint URL: http://localhost:8080/api/chat
- Method: POST 
- Body: JSON containing the query text. 

