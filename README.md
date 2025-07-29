# AI-CHATBOT-WITH-NLP
*COMPANY*: CODTECH IT SOLUTIONS 
*INTERN ID*: CT04DH786
*NAME*: NEHA NITIN BANKAR 
*DOMAIN*: PYTHON 
*DURATION*: 4 WEEKS 
*MENTOR*: NEELA SANTOSH 

#DESCRIPTION:

This Python code creates a simple rule-based chatbot using the Natural Language Toolkit (NLTK) library. The chatbot operates by matching user inputs with predefined patterns and responding with associated replies. The code primarily utilizes NLTK's Chat module from nltk.chat.util, along with reflections, which provides a simple dictionary for reflecting pronouns like "I" to "you", though in this code, reflections are not extensively used.

The heart of the chatbot is the pairs list, which contains tuples of regular expression patterns and corresponding responses. Each pair defines a possible user input pattern and the bot's reply. For example, if a user types "my name is Neha", the bot matches it to the pattern r"my name is (.*)" and responds with "Hello Neha, how can I help you today?". Some patterns like greetings ("hi", "hello", "hey") are grouped together, and the bot randomly selects a response from the list. There's also a catch-all pattern r"(.*)" at the end, ensuring the bot has a default reply when no other pattern matches.

The chatbot() function initializes the chat session. It prints a welcome message and then creates a Chat object with the defined pairs and reflections. The method chat.converse() starts an interactive loop where the bot continuously takes user input and provides appropriate responses based on the pattern matches.

Before starting the chatbot, the code checks if certain NLTK resources (wordnet and punkt) are downloaded. These resources are essential for text processing tasks in many NLTK applications, though they are not directly used in this simple chatbot. If the resources are missing, the code downloads them using nltk.download() to avoid runtime errors.

Finally, the script is executed under the if __name__ == "__main__": block to ensure that it runs only when the file is executed as a standalone program and not when imported as a module elsewhere. This chatbot is purely pattern-based and does not involve machine learning or AI models; hence, its responses are limited to the predefined patterns and lack contextual understanding or memory. Despite its simplicity, it demonstrates the foundational concept of how chatbots function using pattern recognition techniques.




