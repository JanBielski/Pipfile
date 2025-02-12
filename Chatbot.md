import random

responses = {
    "hello": "Hi there! How can I help you?",
    "how are you": "I'm just a bot, but I'm doing fine!",
    "bye": "Goodbye! Have a great day!",
    "default": "I'm not sure I understand that."
}

def chatbot():
    while True:
        user_input = input("You: ").lower()
        if user_input == "exit":
            print("Bot: Goodbye!")
            break
        print("Bot:", responses.get(user_input, responses["default"]))

chatbot()
