# Mobile-Architect-Programming
# Event-Tracking App

Briefly summarize the requirements and goals of the app you developed. What user needs was this app designed to address?
The Event-Tracking App provides a simple and effective platform for users to record, organize, and track events in a minimalistic yet customizable environment. The app was developed to reduce cognitive overload while offering essential features for students, professionals, and event planners.
•	Students can use the app to manage academic tasks like project deadlines and exam dates, focusing on simplicity without unnecessary complexity.
•	Professionals benefit from a tool to track work-related events without needing to sync with external calendars, keeping personal and professional schedules separate.
•	Event planners can organize multiple events efficiently through a user-friendly interface, without the distraction of overly complex features.
Key features of the app include:
•	User authentication for secure account creation and management.
•	A dashboard that displays events chronologically in a grid format.
•	Add, edit, and delete events with a straightforward and easy to use interface.
•	Local data storage via SQLite, ensuring offline access to user credentials and event details.
•	An optional SMS permission flow for sending reminders or notifications.
The app is built to support Android 14 (API level 34) for forward compatibility, while the minimum SDK supported is Android 5 (API level 31), ensuring a broad user base.
The app is free to use and does not include ads or in app purchases at launch. Future monetization options may include a premium version with cloud backup, advanced reminders, and more detailed event categorization.

What screens and features were necessary to support user needs and produce a user-centered UI for the app? How did your UI designs keep users in mind? Why were your designs successful?
The app's user-centered UI was designed with accessibility and ease of use in mind. Key screens and features include:
•	Login/Sign up screen: The login process is straightforward, with a simple form for entering credentials. The interface is designed for quick user access, with minimal input fields.
•	Dashboard: The main dashboard displays events chronologically in a grid layout, with each event displayed clearly to provide quick access to important information. 
•	Event creation and modification screen: This screen allows users to add, edit, and delete events. The interface is designed to be as intuitive as possible, allowing users to enter event details quickly. Once an event is saved, users are returned to the dashboard, maintaining a smooth flow without unnecessary steps.
•	SMS screen: This allows users to enable SMS permissions for event reminders.

How did you approach the process of coding your app? What techniques or strategies did you use? How could those techniques or strategies be applied in the future?
The development process was focused on creating a modular, scalable architecture. I utilized several techniques to ensure the app was well structured, maintainable, and easy to expand in the future:
• Object-Oriented Programming (OOP): Applied OOP principles to keep the codebase organized and modular. Components such as event management, user authentication, and database interactions were built as separate classes. 
• Model-View-Controller (MVC): Implemented the MVC design pattern to clearly separate the app’s logic, data, and user interface. The Model handled SQLite database interactions, the View managed what users saw on screen, and the Controller acted as a bridge between them. This separation made it easier to update the user interface or data handling independently without affecting the rest of the app.
• Asynchronous Programming: Used asynchronous techniques to perform SQLite database operations in the background. This ensured that when the app saved or retrieved event data, the user interface remained responsive. For example, event lists could load while users continued to navigate the app, preventing UI freezing and improving the overall user experience.


How did you test to ensure your code was functional? Why is this process important, and what did it reveal?
Testing was crucial in ensuring that the app functions as expected. It included:
•	Unit Testing: Validated individual components to ensure each feature worked independently.
•	UI Testing: Automated UI tests checked the layout, button responsiveness, and overall functionality on different screen sizes and orientations, ensuring consistency.

Consider the full app design and development process from initial planning to finalization. Where did you have to innovate to overcome a challenge?
One key challenge during development was creating a lightweight yet effective event categorization system that would cater to different user groups (students, professionals, event planners). 
Another challenge was implementing SMS permissions in a way that felt seamless and non-intrusive. The SMS permission screen appears once after login, and users can continue using the app without granting permission. This approach provides clarity about why the permission is requested while ensuring users can make an informed decision without feeling pressured to accept it.

In what specific component of your mobile app were you particularly successful in demonstrating your knowledge, skills, and experience?
I am particularly proud of the user interface (UI) design and the local data storage implementation. By focusing on simplicity and a smooth user flow, I was able to create an app that is both functional and user-friendly, minimizing cognitive load and enhancing overall usability.

A key technical achievement was the development of the DatabaseManager class, which neatly encapsulates all SQL statements within a clean, external API accessible to the rest of the app. This design not only improves code organization and maintainability but also demonstrates my ability to apply sound software engineering principles in practice.

The use of SQLite for local data storage ensures that the app remains fully functional offline, providing users with reliable access to their events without requiring a constant internet connection. Additionally, the event management system (which allows users to efficiently add, edit, and delete events) highlights my skill in creating seamless and intuitive user experiences that help users stay organized without feeling overwhelmed.
