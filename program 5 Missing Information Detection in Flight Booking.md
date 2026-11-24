Travel Booking Data Collection Assistant
https://gemini.google.com/app/cd78635adbe30630

User prompt: A travel booking system collects flight details from customers through natural-language messages. Before processing a booking, the system must verify whether all mandatory information has been provided. Your task is to that extract the available information, identify missing fields, and ask the customer to provide the missing details. Required fields are: - Passenger Name: If missing "Please provide the passenger's name or if multiple passenger's names" - Departure City: If missing "Please provide the departure city" - Destination City: If missing "Please provide the destination city" - Travel Date: If missing "What is the preferred travel date?" - Number of Passengers: If missing "How many passenger's will be travelling?" - Travel Class: If missing "Which travel class do you prefer: Economy, Premium Economy, Business, or First Class?" Additional requirements: 1. Properly extract all the information provided by the customer 2. Never assume or invent missing information 3. Identify all missing mandatory fields 4. Ask relevant questions to collect the missing information 5. If all mandatory information is provided, respond: "All required information has been provided" 6. Do not ask the customer to repeat information already provided. 7. Cases where the exact departure city or destination city hasnt been provided example: Moscow is located both in Russia and USA that is ( Moscow, Kansas; Moscow, Idaho) in such cases prompt the user "Which Destination or Departure city do u mean? Please specify the state or country" Input: "I am Mahesh, I want to book a flight from Bangalore to Hyderabad" Expected output: Passenger Name: Mahesh Departure City: Bengaluru Destination City: Hyderabad Travel Date: Missing Number of Passengers: Missing Travel Class: Missing Please provide the following missing information: 1. What is your preferred travel date? 2. How many passengers will be travelling? 3. Which travel class do you prefer: Economy, Premium Economy, Business, or First Class? objective: to act as an intelligent data-collection assistant, ensuring all mandatory information is available before proceeding with a booking. I will provide the input now
Response: Understood. I am ready to act as your travel booking data-collection assistant, following all your extraction rules, city-disambiguation checks, and output formatting guidelines.
Please share the customer's input whenever you're ready.

User prompt: "I am Rahul. I want to book a flight from Bengaluru to Delhi."
Response: Passenger Name: Rahul Departure City: Bengaluru Destination City: Delhi Travel Date: Missing Number of Passengers: Missing Travel Class: Missing
Please provide the following missing information:
What is the preferred travel date?
How many passengers will be travelling?
Which travel class do you prefer: Economy, Premium Economy, Business, or First Class?

User prompt: "I'm Neha. Book a flight from Chennai to Mumbai on 15th December. Actually, make it 18th December. Two passengers in Economy."
Response: Passenger Name: Neha Departure City: Chennai Destination City: Mumbai Travel Date: 18th December Number of Passengers: 2 Travel Class: Economy
All required information has been provided.

User prompt: "My name is Ajay. I need a flight from Delhi to Goa on 20th December for 2 passengers. Actually, we are 4 people. Economy class."
Response: Passenger Name: Ajay Departure City: Delhi Destination City: Goa Travel Date: 20th December Number of Passengers: 4 Travel Class: Economy
All required information has been provided.

User prompt: "I am Divya. I want to travel from Mumbai to Hyderabad on 15th December with 2 passengers in Luxury Class."
Response: Passenger Name: Divya Departure City: Mumbai Destination City: Hyderabad Travel Date: 15th December Number of Passengers: 2 Travel Class: Missing (Invalid class provided: "Luxury Class")
Please provide the following missing information:
Which travel class do you prefer: Economy, Premium Economy, Business, or First Class?

User prompt: "I'm Aman. Book a flight from Pune to Delhi on 10th December for zero passengers in Economy."
Response: Passenger Name: Aman Departure City: Pune Destination City: Delhi Travel Date: 10th December Number of Passengers: Missing (Invalid count provided: "zero") Travel Class: Economy
Please provide the following missing information:
How many passenger's will be travelling?

User prompt: "I am Rahul. I want to travel from Delhi to Springfield on 12th December for 2 passengers in Economy."
Response: Passenger Name: Rahul Departure City: Delhi Destination City: Missing (Ambiguous city provided: "Springfield") Travel Date: 12th December Number of Passengers: 2 Travel Class: Economy
Please provide the following missing information:
Which Destination or Departure city do u mean? Please specify the state or country.

User prompt: "I need a flight to Bangalore for 3 people."
Response: Passenger Name: Missing Departure City: Missing Destination City: Bengaluru Travel Date: Missing Number of Passengers: 3 Travel Class: Missing
Please provide the following missing information:
Please provide the passenger's name or if multiple passenger's names
Please provide the departure city
What is the preferred travel date?
Which travel class do you prefer: Economy, Premium Economy, Business, or First Class?

