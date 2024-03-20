# Plan for `Smart School Administrative System`

### Customer:
School administration (SHS)

### Issue:
Underutilization of modern technology, more specifically AI in school administration

### Solution:
Smart School Administrative System


### Objectives
- Use ML to automate as many school administrative tasks as possible
    - Tasks:
        - Instant Attendance tracking
        - Student emotion tracking
        - Student management
        - Staff management
        - Finance management

- Gain insights from collected data using ML
    - Include:
        - Grade prediction
        - Financial trends
        - Finance forecast
        - Teacher performance
        - Student performance
        - Career suggestions from student performance


### Objectives Breakdown
1. #### Attendance Tracking:
    Utilize object detection and facial recognition to instantly mark attendance for students.
    We seek to implement a tool that allows teachers to use their phones or any available camera to instantly track attendance simply by directing the camera at the students.
    <br>
    Ideally, this tool should:
    1. Work even with cameras of very low resolutions
    1. Quickly detect, identify and mark student attendance with as little delay as possible in between. (a maximum of 10 seconds to complete).
    1. Accurately identify students with close to zero false positives and true negatives.

1. #### Student Emotion Tracking:
    Utliize a model that has been trained to detect emotions such as happiness, sadness, anger from the facial expression of people to monitor students' emotional status during teaching. This tool should work in realtime and keep collection data on each student and eventually calculate an some engagement index the end of a lesson.
    There should be very little to no lagging between frame captures

1. #### Student Management:
    Centralized storage for all student information using application's database. The application would also provide an interface to observe and make edits to student information.
    This interface should be clear and easy to use. More relevant features should be easy noticed on page load and making edits should be as easy as selecting the value for a particular feature.

1. #### Staff Management:
    Centralized storage and management for teachers and other staff members.

1. #### Finance Management:
    Record keeping of the schools finances and transaction history. As well as a feature that allows for budget allocation and tracking.
    Features:
    - automatic deduction of predetermined expenses such as salaries and indicate the funds available for spending.
    - Statistical financial information, such as average expenditure per term as well as analysis breakdown on the various fields spent on such as average expenditure per infrastructural improvement.
    such data can be used to give more insights into secrets behind school's performance.

1. #### Grade Prediction:
    Using historical student performance information collected over time, accurately predict the future grades of students. Every time a teacher or administrator previews a students information, statistical information about the student's likely future performance should be displayed as well. 
    - This information should be precalculated and only recalculated at intervals (for instance, if the available dataset grows by some factor). 
    - The precalculated value should be stored in a database for easy access.
    - The confidence interview of the prediction should also be displayed

1. #### Teacher Performance Prediction:
    Teacher performance prediction from historical student performance data.
    - quantify teacher performance using some metric, eg(average score over all students in the class)
    - use historical data to predict that metric
    - indicate confidence interval of prediction

1. #### Timetable generation:
    Use historic data to generate efficient timetables that ensure balance and maximize performance in subject fields




### Overall Performance Objective of Application
- #### Speed:
    The application will make use of a lot of data and hence would require many server request, almost every page would require a server request. Hence to avoid situations where users have to wait for long periods before getting any content, the pages must be optimized to reduce their load times.

- #### Security:
    Given that the applications database would hold sensitive information about students, teachers, parents and administrators, as well as the schools financial information, it must be ensured that the data is properly protected from unauthorized access.

- #### Responsiveness:
    The app should be usable on a wide range of devices hence the interface must be able to resize appropriately for different resolutions.

- #### Easy Data Upload:
    The app should allow for easy update of database with csv files (such as csv files for students)


### Application flow
#### Administrator:
- Registration
    - Signs up for school
    - unique id generated for school
    - adds staff and students to the database
    - links to school bank account
- Usage:
    - monitor and edit students
    - monitor and edit staff
    - notify parents through email and sms
    - generate time table
    - generate report cards
#### Teacher:
- Usage:
    - take attendance
    - monitor student emotion


### Application Architecture
1. #### Frontend
1. #### Server
1. #### Database
1. #### ML APIs