# 💻 PDF Query Assistant🤖: RAG model based conversational Interface with Vertex AI and Pinecone
Quote:*"Talent wins games,but teamwork and intelligence wins championships."* ~Michael Jordan
## Project Description
PDF query assistant that leverages cutting-edge technologies to facilitate dynamic conversations with a language model. The project integrates LangChain, Vertex AI, and Pinecone to provide users with an intelligent and responsive conversational experience.

#### Features
* __Conversational Interface__: Engage in natural language conversations with the AI model through a user-friendly Streamlit chat interface.
* __Context-Aware Responses__:The system utilizes LangChain's ConversationChain to maintain context-aware      responses, ensuring coherent and relevant answers based on the conversation history.
*  __Powerful Embeddings__: The project harnesses the capabilities of Vertex AIEmbeddings to generate powerful embeddings for both queries and historical conversations.
* __Efficient Indexing__: Pinecone is employed to index and retrieve relevant information efficiently, enhancing the speed and accuracy of responses.

 

 ## Dependencies
 * [LangChain](https://python.langchain.com/docs/get_started/introduction)
 * [Vertex AI](https://cloud.google.com/vertex-ai?hl=en)  Prerequisite:(Required a active GCP account and Project Id)
 * [Pinecone](https://docs.pinecone.io/docs/overview)
 * [Streamlit](https://docs.streamlit.io/)
 * [Google Cloud Platform](https://cloud.google.com/free?utm_source=PMAX&utm_medium=PMAX&utm_campaign=FY24-H1-apac-gcp-DR-campaign-IN&utm_content=in-en&gad_source=1&gclid=Cj0KCQiAwbitBhDIARIsABfFYIIlUTt1r3N7jb_O-P0O30PhmkFmTNyaEnJUy6QPExzqk6iie0Rq7OAaAuzCEALw_wcB&gclsrc=aw.ds&hl=en)

 ## How to Install and Run the Project
 * Clone the repository:
    ```bash
    git clone https://github.com/your-username/pdf-interacter.git
    ```
*  Activate the existing Virtual Environment:
    ```bash
    source venv/bin/activate
    ```
*  Install Dependencies:
    ```bash
    pip install -r requirements.txt
    ```
*   Create a Service Account Key:
    * Go to the Google Cloud Console: https://console.cloud.google.com/
    * Navigate to the project for which you want to create credentials.
    * In the left navigation pane, click on "IAM & admin" and then "Service accounts."
    * Click on the service account for your project.
    * In the "Keys" tab, click on "Create key," and choose JSON as the key type.
    * Save the JSON file with the service account key securely.

*  Download a service account credentials file (eg:<file_name>.json)
<br>
        Set the GOOGLE_APPLICATION_CREDENTIALS Environment Variable: Ensure that the GOOGLE_APPLICATION_CREDENTIALS environment variable is set to the path of your service account key JSON file. 
    ```bash
    export GOOGLE_APPLICATION_CREDENTIALS="/path/to/your/service-account-key.json"
    ```

*   Set the API key and Environment details:
    * main.py
    ```bash
    PINECONE_API_KEY = ""
    PINECONE_API_ENV = ""
    PINECONE_INDEX_NAME = ""
    # Explicitly set credentials using service account key
    creds = service_account.Credentials.from_service_account_file(
    '/path/to/your/service-account-key.json',
    scopes=['https://www.googleapis.com/auth/cloud-platform']
    )
    # Set the project ID (replace 'your-project-id' with your actual GCP project ID)
    project_id = ''
    ```
* Run the project in terminal:
    ```bash
    python main.py
    streamlit run web.py
    ```

## Purpose of the project
This project is solely for demonstration.It includes basic overview how a llm model works in case of text with integration of Pincone as a vectordatabase and VertexAI as a model.
The purpose of the project is to create an interactive PDF query assistant that utilizes state-of-the-art technologies to enable dynamic and context-aware conversations with a language model. The project serves several key purposes:

* __Conversational Interface__: Provide users with a natural language interface for interacting with a language model. The Streamlit chat interface makes it user-friendly, allowing users to input queries and receive responses in a conversational manner.

* __Context-Aware Responses__: Implement a system that maintains context-aware responses. The LangChain ConversationChain is employed to ensure that the AI model understands and responds coherently based on the history of the conversation.

* __Embeddings for Enhanced Understanding__: Utilize advanced embeddings generated by Vertex AIEmbeddings to enhance the understanding of both user queries and historical conversation context. This improves the model's ability to generate meaningful and relevant responses.

* __Efficient Information Retrieval__: Implement efficient information retrieval using Pinecone. The system indexes relevant information, allowing for quick and accurate responses to user queries by leveraging powerful indexing and retrieval mechanisms.

* __Demonstrate Integration of Technologies__: Showcase the integration of various technologies, including LangChain, Vertex AI, and Pinecone. The project demonstrates how these technologies can work together seamlessly to create an intelligent conversational system.

* __Explore Conversational AI Capabilities__: Enable users to explore the capabilities of conversational AI in the context of PDF documents. The project aims to make interactions with PDF documents more intuitive and efficient through natural language conversations.

* __Open Source Contribution__: Provide an open-source project that welcomes contributions from the community. Users can contribute by submitting issues, feature requests, or pull requests to enhance and expand the functionality of the  project.

Overall, the  project serves as a practical and educational example of integrating advanced technologies to create a conversational AI application with real-world applications in document interaction and information retrieval.

## Contributing to this Project
 * __Reporting Bugs__: If you find a bug, please ensure that it hasn't already been reported. If not, open a new issue providing as much detail as possible, including the steps to reproduce the bug.
 * __Suggesting Enhancements__:If you have an idea for an enhancement, open an issue outlining your proposal. Be sure to include details about the suggested feature and how it would improve the project.
* __Pull Requests__:
    * Fork the repository and create your branch from main.
    * Test your changes thoroughly.
    * Commit your changes with clear and descriptive commit messages.
    * Push your branch to your fork and submit a pull request.
    * Ensure that your pull request is linked to an existing issue or create a new issue for it.
    * Your pull request will be reviewed, and further adjustments may be requested before merging.

## Contact us:
* Email-Id: codingshubham.in@gmail.com
* Email-Id: yashmukherjee62@gmail.com





