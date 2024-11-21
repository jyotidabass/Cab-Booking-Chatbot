# Cab-Booking-Chatbot

Here is a line-by-line explanation of the code:
1. import nltk
This line imports the Natural Language Toolkit (NLTK) library, which is a popular library used for Natural Language Processing (NLP) tasks.

2. from nltk.stem import WordNetLemmatizer
This line imports the WordNetLemmatizer class from the NLTK library, which is used for stemming and lemmatization of words. However, in this code, this import is not used.

3. lemmatizer = WordNetLemmatizer()
This line creates an instance of the WordNetLemmatizer class, but as mentioned earlier, it is not used in this code.

4. import random
This line imports the random library, which is not used in this code.

5. cabs = [...])
This line defines a list of dictionaries, where each dictionary represents a cab with its id, name, and availability.

6. booking_details = {}
This line defines an empty dictionary to store the user's booking details.

7. def book_cab():
This line defines a function named book_cab that contains the main logic of the chatbot.

8. print("Welcome to Cab Booking Chatbot!")
This line prints a welcome message to the user.

9. print("Please type 'book' to book a cab or 'exit' to quit.")
This line prints instructions on how to use the chatbot.

10. while True:
This line starts an infinite loop that will continue until the user types 'exit'.

11. user_input = input("You: ")
This line gets the user's input from the console.

12. user_input = user_input.lower()
This line converts the user's input to lowercase to make the chatbot case-insensitive.

13. if user_input == "book":
This line checks if the user's input is 'book'.

14. print("Please enter your pickup location:")
If the user's input is 'book', this line prints a prompt to enter the pickup location.

15. pickup_location = input("You: ")
This line gets the user's pickup location from the console.

16. print("Please enter your destination:")
This line prints a prompt to enter the destination.

17. destination = input("You: ")
This line gets the user's destination from the console.

18. print("Which cab type do you prefer? (Uber/Ola/TaxiForSure)")
This line prints a prompt to select the preferred cab type`.

19. cab_type = input("You: ")
This line gets the user's preferred cab type from the console.

20. for cab in cabs:
This line starts a loop that iterates through the cabs list.

21. if cab["name"].lower() == cab_type.lower() and cab["available"]:
This line checks if the user's preferred cab type is available.

22. booking_details["cab_id"] = cab["id"]
If the cab is available, this line stores the cab id in the booking_details dictionary.

23. booking_details["pickup_location"] = pickup_location
This line stores the pickup location in the booking_details dictionary.

24. booking_details["destination"] = destination
This line stores the destination in the booking_details dictionary.

25. cab["available"] = False
This line updates the availability of the cab to False.

26. print(f"Cab {cab_type} booked successfully!")
This line prints a success message.

27. print("Your booking details:")
This line prints a header for the booking details.

28. print(booking_details)
This line prints the booking details.

29. break
This line breaks out of the loop.

30. else: print("Sorry, your preferred cab type is not available.")
If no cab is available, this line prints an error message.

31. elif user_input == "exit":
This line checks if the user's input is 'exit'.

32. print("Thank you for using our chatbot!")
This line prints a farewell message.

33. break
This line breaks out of the loop.

34. else: print("Sorry, I didn't understand that. Please try again.")
If the user's input is neither 'book' nor 'exit', this line
