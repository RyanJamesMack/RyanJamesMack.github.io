Vision Statement
---------
UStep is an academic application designed to help students track their current course grades, predict their final grades based on input, and view and add course reviews for courses offered by their department.

Intended Users
---------
The UStep app will serve as an educational and user-friendly tool designed to streamline academic performance for students at the University of Manitoba. This app will assist users in planning their course journey by providing an interactive experience that manages their progress toward achieving good grade in a course. Students will be able to register/sign in with their email, and password, further specifying their major degree and year of study. Based on this information, the app will create a course catalogue, which will automatically fetch the courses offered by the specified major department. Moreover, students will be able to add or remove from the list their past and current courses.

Major Functionality
---------------
- Signup/Login (UI & Database)
- User Profile Setup (UI & Database)
- Course Catalog Management (UI & Database)
- Course Review (UI & Database)
- Settings (with logout and Dark Mode)
- Grade Tracker (UI & Database)

Team Members Development Takeaways
------------
### Hoang Huy Truong - Learning Outcome
Throughout the development process, I had opportunities to interact Mockito and AndroidJUnit4 testing frameworks and gained valuable experience on writing effective unit, integration and system tests, understanding the importance of test driven development technique. Additionally, I also learned how to utilize and promote three layer architecture, which is commonly used by many systems nowadays, to build entire application.

### Ryan Mack - Learning Outcome
The biggest thing that I learned from working on the UStep app is how to use Android Studio to build and debug android apps. This gave me experience working with a common software, as well as experience working and understanding a very large software project. It also made me more familiar with using version control software like git to manage my work.

### Subhash Yadav - Learning Outcome
Through the development of the UStep application, I gained hands-on experience in designing and implementing core functionalities such as grade tracking and user authentication. I deepened my understanding of UI development, and API integration while working on grade prediction. Additionally, collaborating with a team helped me refine my communication and project management skills, enhancing my ability to work in a structured development environment.

### Hai Dang Nguyen - Learning Outcome
I personally learned how to use HSQLDB for lightweight database integration, how to build and debug Android apps using Android Studio, and how to write effective tests using JUnit and Mockito for both unit and Integration testing.

### Shaheer Ansari - Learning Outcome
Working on the features helped me understand the importance of consistent testing in ensuring reliable  workflow. I gained hands-on experience with JUnit , architecture management, and activity lifecycle handling, while also learning how to debug and fix issues related to the database and it's relation with the our logic layer.

Screen Recording
------

<iframe width="560" height="315" src="https://www.youtube.com/embed/3Lqz4Q15VPA?si=HcHs7v8wngn1wuMJ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

Postmortem
---------
### What took the most time? The least? Any surprises?
During the development process, we encountered significant difficulties connecting to the database and faced unexpected issues after establishing the connection. Resolving these problems took us about three weeks, making it the most time-consuming challenge we faced. The database connection issue was also the most surprising issue throughout progress.
In Iteration 2, we were required to ensure that every feature operated with the actual database running underneath. However, we underestimated the importance of early database setup and only started configuring it a few days before the deadline. This led to unexpected connection issues, which disrupted multiple database-dependent features and prevented them from activating. As a result, we lost a substantial number of marks in Iteration 2.
On the other hand, the least time-consuming task was the establishment of domain-specific objects. This process was fairly straightforward since it only involved identifying appropriate fields for each object and constructing them using constructors, along with getters and setters for every field.

### Are there any particular design smells, or brilliant design decisions?
One major design smell was the violation of the Single Responsibility Principle (SRP) and Separation of Concerns (SOC) in several Data Storage Objects (Assessment.java, Course.java, StudentCourse.java). These classes were not only responsible for storing and retrieving data but also contained setter methods that managed logic, which should ideally be handled in a separate service layer. This made the code harder to maintain and scale, as changes to business logic would require edits across multiple classes.

### What did you learn about team or large project development? What will you start doing, keep doing, or stop doing next time?
One of the most valuable lessons we learned from working on a large-scale project was the importance of frequent and effective communication within the team. In particular, when it came to committing and pushing changes to major branches such as develop, there were no clear restrictions on when to push to it, and we often failed to notify other members regarding latest commits. Consequently, some team members were unaware of the latest changes and did not pull the updates, leading to significant merging conflicts and integration issues later.
In order to address this, we realized the need for more frequent updates on project tasks and proactive communication when encountering difficulties. Moving forward, every team member should provide regular status updates and seek support whenever necessary. Additionally, any commit or decision that could significantly impact the project must be thoroughly discussed and agreed upon by the entire team before execution. Implementing these changes will help prevent misunderstandings, reduce conflicts, and create a more unified workflow.

