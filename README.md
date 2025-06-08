def chatbot():
    responses = {
        "hi": "Hello! How can I help you today?",
        "hello": "Hi there! Need support with something?",
        "help": "Sure, I can help. Please describe your issue.",
        "pricing": "Our pricing depends on the service. Can you specify?",
        "services": "We offer data analysis, ML model support, and tutoring.",
        "bye": "Goodbye! Have a great day.",
        "thanks": "You're welcome!",
        "reset password": "To reset your password, visit our website,
        "contact": "You can email us at support@yyy.com",
    }
    print("SupportBot: Hello! Type 'bye' to exit")
    while True:
        user_input = input ("You:").lower().strip()
        if user_input == "bye":
            print("SupportBot: Bye!")
            break
        response = responses.get(user_input, "SupportBot: Sorry, I don't understand that.")
        print(response)

if __name__ == "__main__":
    chatbot()
