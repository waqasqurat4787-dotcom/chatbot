def chatbot_response(user_input):
    user_input = user_input.lower()

    if user_input == "hello":
        return "Hi there!"
    elif user_input == "how are you":
        return "I am fine, thanks!"
    elif user_input == "bye":
        return "Goodbye!"
    else:
        return "I don't understand."

print("Chat Bot Started! Type 'bye' to exit.\n")

while True:
    text = input("You: ")
    print("Bot:", chatbot_response(text))
    
    if text.lower() == "bye":
        break
