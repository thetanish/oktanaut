<p align="center">
  <img src="https://github.com/tanishkumar02/oktanaut/assets/144177229/5dac993d-8344-47d3-8611-15ca7a06e9e6"/>
</p>

In today's fast-paced world of technology, developer support is essential to ensure a seamless experience for users navigating intricate platforms and APIs. As a Developer Support Intern at Okta, I embarked on a challenging yet rewarding endeavor to create a solution that would streamline accessing and comprehending the Okta developer documentation. The result of my efforts is :sparkles:Oktanaut:sparkles:, a versatile chatbot built in Python, designed to assist users in harnessing the power of Okta's developer documentation, available at developer.okta.com.
The chatbot is built using the GPT-3.5 Turbo model from OpenAI and displayed in a web interface created with the Python panel library.
Here's a step-by-step walkthrough of how the code works and how to use it:
1. Library installation: The script begins with installing the required Python packages: [OpenAI](https://pypi.org/project/openai/), [Panel](https://panel.holoviz.org/getting_started/installation.html), and [LlamaIndex](https://pypi.org/project/llama-index/). These packages work with the GPT-3.5 model, create the web interface, and manage the chatbot's conversation.
2. Get an OpenAI API key by creating an account and following the instructions at https://help.openai.com/en/articles/4936850-where-do-i-find-my-api-key. Replace the API Key code snippet with your API Key
4. Download the files from https://drive.google.com/drive/folders/11W-cjmkTztmnGgJCsJRtE395Iji6JX53?usp=share_link and make sure the files are saved on your drive (not within any folders) and you are mounting the files from the correct account
5. continue_conversation: This function takes a list of messages as input and continues the conversation with the GPT-3.5 Turbo model. It sends the messages to the model and receives a response.
    - model="gpt-3.5-turbo": Specifies the GPT-3.5 Turbo model for conversation.
    - messages: The list of messages that make up the conversation.
    - temperature: A parameter that controls the randomness of the model's responses.
6. add_prompts_conversation: This function adds prompts to the conversation and retrieves responses from the chatbot. It's triggered by clicking on the web interface.
7. The user enters a prompt in the client_prompt input field.
8. The user's input is added to the conversation with the role "user."
9. The continue_conversation function is called to get the chatbot's response.
10. The chatbot's response is added to the conversation with the role "assistant."
11. context list: This list initializes the conversation with a system message that introduces Oktanaut, the chatbot. It provides information about the bot's purpose and capabilities.
12. pn.extension(): This line initializes the Panel extension, enabling the creation of the web-based user interface.
13. panels list: This list will store the components displayed in the web interface.
14. client_prompt input field: This widget allows users to input their questions or prompts for Oktanaut.
15. button_conversation: This is the button to submit the user's question and trigger the conversation with Oktanaut.
16. interactive_conversation function binding: This line binds the add_prompts_conversation function to the button_conversation button, making it interactive and responsive to user input.
17. dashboard layout: This section assembles the user interface, including the input field, the conversation button, and the chatbot's responses.

Now, here's how to use the code:
1. Run the Python script in your development environment.
2. After running the script, a web interface will be displayed, including an input field and a "Chat with Oktanaut!" button.
3. Enter your questions or prompts in the input field. For example, you can ask about Okta or OAuth developer documentation.
4. Click the "Chat with Oktanaut!" button to submit your question.
5. Oktanaut will respond to your question with a chatbot-generated answer.
6. You can continue the conversation by entering additional questions or prompts and clicking the button.
7. To end the session, you can say "thank you," as mentioned in the introductory message.
8. The chatbot will answer questions and converse based on your prompts. It uses the GPT-3.5 Turbo model to generate responses.

Note: The conversation and responses will appear on the web interface in real-time.
The web interface allows you to have interactive conversations with Oktanaut and receive answers to your questions about Okta and OAuth         developer documentation. Feel free to try it out and have a conversation with Oktanaut!![oktanaut (1)]

