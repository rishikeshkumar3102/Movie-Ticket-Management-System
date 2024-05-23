This project aims to design and implement an MTMS using a DBMS that 
effectively manages the entire lifecycle of movie ticket sales, from ticket 
booking to seat allocation and reporting. The system should cater to the needs of 
both customers and theater administrators, providing a user-friendly interface 
for seamless interaction and management.
Requirement Collection 
 
Users should be able to register with the system by providing their first name, 
last name, email, age, and phone number. User IDs (Web_User_ID) should be 
automatically generated or assigned during registration. The system must 
enforce the uniqueness of email IDs and Web User IDs. User information 
should be securely stored in the database. 
 
The system should support the addition of new theatres, each identified by a 
unique Theatre_ID. Theatre details, including the name, the number of screens, 
and the area, must be captured and maintained. The theatre name should be 
mandatory and unique. 
 
Screens should be associated with a specific theatre (Theatre_ID).The system 
must track the number of seats in both Gold and Silver classes for each screen. 
Deleting a theatre should automatically delete associated screens (ON DELETE 
CASCADE). 
 
Movies must be added to the system with a unique Movie_ID. Movie details 
such as name, language, genre, and target audience should be recorded. 
 
Shows should be scheduled with unique Show_IDs, specifying show times, 
dates, and remaining seat availability. Each show should be associated with a 
specific screen (Screen_ID) and a movie (Movie_ID). Class costs for both Gold 
and Silver classes should be recorded. 
 
Bookings should be made for specific shows (Show_ID) by users (User_ID). 
Each booking is identified by a unique Booking_ID. The system should record 
the number of tickets, total cost, and payment details (Card_Number, 
Name_on_card). 
 
Tickets are associated with a specific booking (Booking_ID). Each ticket has a 
unique Ticket_ID, specifying the class (Gold/Silver) and price. 
