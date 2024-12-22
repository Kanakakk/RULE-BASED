# RULE-BASED# Advanced Interactive Chatbot with more responses and follow-up questions
def chatbot():
    print("Hi, I'm Chatbot! Type 'bye' to end the conversation.")
    
    # Asking user's name
    user_name = input("Chatbot: What's your name? ")
    print(f"Chatbot: Nice to meet you, {user_name}!")
    
    # Ask how the user is doing
    user_feeling = input(f"Chatbot: How are you feeling today, {user_name}? ").lower()
    if user_feeling in ["good", "great", "awesome", "fine"]:
        print("Chatbot: That's awesome! I'm happy to hear that.")
    elif user_feeling in ["bad", "not good", "sad"]:
        print("Chatbot: I'm sorry to hear that. I hope your day gets better!")
    else:
        print("Chatbot: I see! Thanks for sharing how you're feeling.")

    while True:
        # Take user input
        user_input = input(f"{user_name}: ").lower()  # Convert to lowercase
        
        # Exit condition
        if user_input == "bye":
            print("Chatbot: Goodbye! It was nice chatting with you.")
            break
        
        # Respond to various queries
        elif user_input == "hello":
            print("Chatbot: Hi there! How can I help you today?")
        
        elif user_input == "how are you":
            print("Chatbot: I'm just a program, but I'm doing great! How about you?")
        
        elif user_input == "what is your name":
            print("Chatbot: I'm Chatbot! What's your name again?")
        
        elif user_input == "how old are you":
            print("Chatbot: I don't have an age, but I was created recently to chat with you!")
        
        elif user_input == "what can you do":
            print("Chatbot: I can talk to you, answer questions, tell jokes, and even play some trivia!")
        
        elif user_input == "tell me a joke":
            print("Chatbot: Why don't skeletons fight each other? They don't have the guts!")
        
        elif user_input == "what is the weather like":
            print("Chatbot: I don't know the exact weather, but I hope it's nice where you are!")
        
        elif "your favorite" in user_input:
            print("Chatbot: I don't have favorites, but I think all things tech are pretty cool!")
        
        elif user_input == "do you like music":
            print("Chatbot: I don't listen to music, but I know a lot about it! Do you have a favorite genre?")
        
        elif user_input == "tell me a fun fact":
            print("Chatbot: Did you know? Octopuses have three hearts!")
        
        elif user_input == "how do I make a sandwich":
            print("Chatbot: Making a sandwich is easy! Just take two slices of bread and put your favorite filling in between!")
        
        elif user_input == "tell me a riddle":
            print("Chatbot: Alright, here's a riddle for you: What has keys but can't open locks?")

        elif "riddle answer" in user_input:
            print("Chatbot: The answer is a piano! 🎹")
        
        elif user_input == "do you know any trivia":
            print("Chatbot: Sure! Here's a trivia question for you: What is the largest planet in our solar system?")
        
        elif "earth" in user_input:
            print("Chatbot: Earth is awesome, but the largest planet is Jupiter!")
        
        elif user_input == "can you help me with math":
            print("Chatbot: Sure! What kind of math problem do you need help with?")
        
        else:
            print("Chatbot: I didn't quite understand that. Can you ask something else or give me more details?")

# Start the chatbot
chatbot()

