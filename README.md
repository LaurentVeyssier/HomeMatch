# HomeMatch
final project for UDACITY Building GenAI solutions 4 weeks course

# PROJECT DESCRIPTION
The project aims at building a real-estate chatbot able to identify the best properties matching customer preferences.
The project uses OpenAI, langchain and vectorDB.

# PROJECT STEPS
1 - Prepare synthetic property listings\n
2 - Generate property listings embeddings and store in a vector database\n
3 - Identify customer preferences using LLM and pydantic schema
4 - Extract top-k best matches from vector database using distance threshold
5 - Augment the property descriptions and personalize the final ouput to the buyer's preferences without altering factual properties' characteristics

# PROJECT SPECIFICITIES
- Step 3 leverages pydantic schemas to extract customer preferences from text input and use for metadata filtering
- Semantic search: Step 4 vectorSearch combines **semantic search** and **metadata filtering** to increase matching capabilities and extend performance
- The project concludes with an end-to-end workflow from customer input to the presentation of the top augmented matches in natural language. The workflow uses tools and function calling to generate the final output.

# PROJECT IMPLEMENTATION
- clone the repo and install the dependencies in a virtual environment. The required libraries are located in the requirements.txt file
- enter your openai api secret key in a .env file to save in the project folder. It will be loaded to your env variables at the start of the notebook
- Execute the notebook in the virtual environment
- You can skip step 1 and step 2 in the notebook and just load the synthetic property listings saved in the folder data
- The folder data contains the vectordb with the associated embeddings
- Query the database modifying the customer input
