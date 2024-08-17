# Vapi-AI-Voice-Assistant

Initial Steps:
1.	Create a Vapi Account:
•	Sign up for an account with Vapi to utilize the no-code AI voice assistant features.
2.	Create an Account on Make.com:
•	Register on Make.com to leverage additional external features and integrations.


Vapi AI Setup:
Step 1: Create a New Voice Assistant
- You can start from a blank slate or choose a template.
- After creating the voice assistant, set up the following:
- First Message: This is used for greeting the user.
- System Prompt: This defines the purpose of the voice assistant and instructs it on how to handle user interactions.

Example:
For an IT company voice assistant designed to book appointments, the First Message might be a friendly greeting, and the System Prompt would explain that the assistant's role is to            help users book appointments.
First Message: Hello, this is Botty from Bot Lab. How can I assist you today?
System Prompt: 
You are a voice assistant for Bot Lab, an IT office located at 123 North Face Place, Anaheim, California. The Office hours are 8 AM to 5PM daily, but they are closed on Sundays.
You are tasked with answering questions about the business, and booking appointments. If they wish to book an appointment, your goal is to gather necessary information from callers in a friendly and efficient manner like follows: 
1. Ask for their full name.
2. Ask for the purpose of their appointment.
3. Request their preferred date for the appointment.
4. Request their preferred time for the appointment.
5. Refuse to book if preferred time is not in office hours
5. Confirm all details with the caller, including the date and time of the appointment.
6. format the date in DD/MM/YYYY
 
Here are some important instructions you need to follow:
1. call the function "check_bookings" only after you get date and time
2. check booking function will give you busy slot so do not book on busy slot
3. When awaiting a response, you might say 'hold on for a moment.'
4. ask user for date and time which do not conflict busy slot
5. call the function "book_the_slot" only when the chosen time do not conflict with busy time and this function needs to be called when you get name and purpose of booking
 
- Be sure to be kind of funny and witty!
- Keep all your responses short and simple. Use casual language, phrases like "Umm...", "Well...", and "I mean" are preferred.
- This is a voice conversation, so keep your responses short, like in a real conversation. Don't ramble for too long.

 ![image](https://github.com/Jiten-Advic/Vapi-AI-Voice-Assistant/assets/169840985/00c02971-98ac-4057-9e5d-2294d40976ae)

	            
Step 2: Create Functions Using the Dashboard Function Option
- Create a function named “Check_bookings” to check appointments on a given date.
- Integrate this function with Vapi by connecting it to a webhook URL from Make.com

 ![image](https://github.com/Jiten-Advic/Vapi-AI-Voice-Assistant/assets/169840985/8e043a85-a450-4646-a12f-4039f20119a9)

- Create a Second function named “Book_the_slot” for book appointments on a given date and time and also take name and purpose of appointment from user.
- Integrate this function with Vapi by connecting it to a webhook URL from Make.com

![Untitled design (2)](https://github.com/Jiten-Advic/Vapi-AI-Voice-Assistant/assets/169840985/0276ef8a-42f6-460c-bc1b-68fab0cdf574)

Step 3: Create Flows in Make.com
- Create the first flow for checking appointments.

 ![image](https://github.com/Jiten-Advic/Vapi-AI-Voice-Assistant/assets/169840985/d6069aed-2ccb-48f5-8bf5-0ada90644793)

- Create the second flow for booking appointments.

![image](https://github.com/Jiten-Advic/Vapi-AI-Voice-Assistant/assets/169840985/6fdfa9d1-3ef5-4a56-a5bc-ad8ef540bf8b)









