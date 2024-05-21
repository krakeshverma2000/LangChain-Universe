### LangChain-Universe

- This GitHub repository is for for integrating OpenAI's API into an application called "Explore Beyond Universe." The code utilizes the langchain library, which provides various functionalities for language processing and conversation management. The application is built using the Streamlit framework.

- The integration starts by setting up the necessary dependencies and environment variables. The user can input a topic of interest through a text input field. The code then utilizes Prompt Templates to generate prompts for conversational interactions. The first prompt asks the user to provide information about a specific object or person. The conversation history related to this input is stored in the person_memory.

- Next, the code employs the OpenAI LLMS (Language Learning Models as Services) to generate a response based on the input. It uses the LLMChain class to manage the conversation flow and store the output related to the object's formation. The conversation history for this input is stored in the dob_memory.

- Following that, the code generates a prompt asking for major events related to the provided object's formation date. The LLMChain class is used again to process the input and store the output in the descr_memory.

- To organize and execute these conversational chains in sequence, the parent_chain is created using the SequentialChain class. It takes the chains for each conversation step and specifies the input and output variables.

- Finally, if the user provides an input text, the parent_chain is executed with the input value, and the results are displayed. The conversation histories for the person's name and major events are shown using expandable sections.

This code serves as a foundation for building conversational AI applications that leverage OpenAI's API and the langchain library for seamless interaction with users.


![Screenshot 2023-06-22 004233](https://github.com/saqib772/LangChain-Universe/assets/121972215/b822a959-1385-4dc9-af94-75ec2611d28d)

