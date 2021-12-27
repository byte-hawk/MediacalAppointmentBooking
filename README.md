**Medical Appointment Booking**

Medical appointment booking is an application for booking appointments for doctors for various specialisations. A patient can use the application to search doctors by specialisations or by city. Once the patient has finalized the doctor, the patient should be able to book an appointment with the doctor for a specific slot.

Following entities will be present in the applications:
- Doctor
- Appointment
- Patient

A doctor should be able to register in the application with the following details of theirs:
- First Name
- Last Name
- Specialization
- Registration Number
- Years of Experience
- Qualification
- Clinic Name

The list of specializations should be already defined at the system level, and the doctors should be able to choose from the list. The doctors should also be able to add multiple booking slots, each containing the following details:
- Start Hour
- End Hour
- Day of week
- Clinic ID

The start and end hour should follow the 24 hour format. The doctors can add their available hours like this: 10(Start Hour -  equivalent of 10 am) to 13(End Hour - equivalent of 1pm) for Monday and then again another booking slot for the same day from 14(Start Hour) to 18(End Hour). The day of week needs to be chosen from a fixed set of values, defined in the system to ensure consistency. 

While the doctors can add their available hours in a range spanning upto 12 hours, the users will be able to book a slot of duration of 1 hour only. The application should keep track of the availability of the doctor for every 60 minute time interval, starting at each hour of the doctor's available time. i.e. if the doctor has added that, he/she will be available from 10am to 12pm in a day, then the users can book an appointment in either of these slots: 10:00am to  11:00am, 11:00am to 12:00pm. Once a user has booked the slot 10:00am to 11:00am on a specific date, the doctor will not be available for another booking in the same time range.

A user should be able to register with the following profile details:
- First name
- Last name
- Contact
    - Email ID
    - Phone
- Address
    - City
    - Locality
    - State
    - Pin Code 

Once the user completes registration, the system should also capture the time, when the user has registered.

A user should be able to search for a doctor by his/her specialisation or city. The user chooses a doctor, the user will be able to book a time slot for a specific doctor for appointment. Once the appointment is booked, the application should print the details of the appointment.

An appointment will capture the following details and should be able to print the details, when required.
- User name
- Doctor name
- Date
- Start Hour
- Clinic Name
- City

User, Doctor & Appointment- each of these entities will also have 2 more attributes:
- Instance level "ID"
- Static variable named "counter", which will be initialized with 0. 

In each object creation, the "ID" attribute will be set as the current value of this variable. And after the object creation, this static variable needs to be incremented by 1. 

<img width="522" alt="Screenshot 2021-12-28 at 2 55 20 AM" src="https://user-images.githubusercontent.com/10265166/147508242-ccd5c564-23ad-4b65-bbad-d778cc602fad.png">
<img width="805" alt="Screenshot 2021-12-28 at 3 11 07 AM" src="https://user-images.githubusercontent.com/10265166/147509003-f22fad8a-37a1-4957-8daa-71e5bd3d3b01.png">
<img width="663" alt="Screenshot 2021-12-28 at 3 17 39 AM" src="https://user-images.githubusercontent.com/10265166/147509322-80b97425-09e0-4fb9-915a-8b8e0bc63b1d.png">
<img width="1674" alt="Screenshot 2021-12-28 at 3 20 37 AM" src="https://user-images.githubusercontent.com/10265166/147509427-5a66d7ca-4a0d-45de-aba5-57bd7690e764.png">
