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

![image](https://github.com/user-attachments/assets/e6aee800-dfd5-44ca-bc59-8f0746322731)


	            
Step 2: Create Functions Using the Dashboard Function Option
- Create a function named “Check_bookings” to check appointments on a given date.
- Integrate this function with Vapi by connecting it to a webhook URL from Make.com

![image](https://github.com/user-attachments/assets/915ebe47-cbed-4066-97fc-ede38051a023)


- Create a Second function named “Book_the_slot” for book appointments on a given date and time and also take name and purpose of appointment from user.
- Integrate this function with Vapi by connecting it to a webhook URL from Make.com

![Untitled design (3)](https://github.com/user-attachments/assets/097aea92-38a3-4bfc-9f0d-8d031901f843)


Step 3: Create Flows in Make.com
- Create the first flow for checking appointments.

![image](https://github.com/user-attachments/assets/d015c0ea-e38f-4a81-b0fa-55dbee17e012)


- Create the second flow for booking appointments.

![image](https://github.com/user-attachments/assets/7826c631-032f-4862-b428-7c1ff2766037)










