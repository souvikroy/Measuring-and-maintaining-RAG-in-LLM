# Maintaining RAGs in LLM
In this work, we use Generative AI LLM modeling techniques to create a project management RAG system tool. RAG is a coloring system that assigns a color (Red, Amber, or Green) to each project task indicating its progress status.

![app_snapshot](https://github.com/souvikroy/Measuring-and-maintaining-RAG-in-LLM/assets/4746631/a4b1649b-6d7c-4680-a548-3a622491956a)
Once the project data is fed into the tool, the LLM model is prompted to provide project management expert recommendation on how to proceed on the task according to its understanding of the data provided.

![recommendation_snapshot](https://github.com/souvikroy/Measuring-and-maintaining-RAG-in-LLM/assets/4746631/89366ebe-38c7-48b2-a2f9-21888d8b4e9f)

# Approach
* Utilizing LangChain open source framwork to create the LLM model
* Using OpenAI API as our prompting channel
* The user interface app is created using Flask web frame

# Requirements
* langchain
* OpenAI
* flask
* Pandas
* pydantic==1.10.8

# Using the app
* The app simplifies the RAG system into evaluating the task status based on the spent budget and the task deadline
* The initial project data is added to the package in csv format and saved as "tasks.csv"
* The user can then start the app by running app.py
* To update a task data, the user can access the editing page by clicking the "Update a task" button
* The user defines the number of the task and the budget already spent on the task to date, and then clicks "Update status"
* The LLM is then automatically prompted to evaluate the task status based on the new data and provides updated expert recommendations
![update_button](https://github.com/souvikroy/Measuring-and-maintaining-RAG-in-LLM/assets/4746631/00858e32-a9ff-4b4d-8e03-6e7728b015c0)
![editing_snapshot](https://github.com/souvikroy/Measuring-and-maintaining-RAG-in-LLM/assets/4746631/a269fd9d-4b65-440e-a3ac-6f633a27b7b7)








