# CODSOFT
Daily Tasks
import random

def chatbot_response(user_input):
    # Predefined responses
    responses = [
        "Hello! How can I help you today?",
        "I'm doing well, thank you for asking!",
        "Goodbye! Have a wonderful day!",
        "I'm sorry, I didn't understand that."
    ]
    
    # Generate a random response
    return random.choice(responses)

# Test the chatbot
print("Welcome to the Random Chatbot! Type 'bye' to exit.")
while True:
    user_input = input("You: ")
    if user_input.lower() == 'bye':
        print(chatbot_response(user_input))
        break
    else:
        print("Chatbot:", chatbot_response(user_input))
