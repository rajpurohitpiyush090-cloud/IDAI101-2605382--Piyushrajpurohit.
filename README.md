# IDAI101-2605382--Piyushrajpurohit.
ParentConnect AI is an AI-powered school communication chatbot developed as part of the Artificial Intelligence: Real-World Applications and Implications course. The project focuses on using conversational AI to improve communication between schools and parents.
In a traditional school environment, parents often need to contact the school office or teachers to obtain basic information such as student attendance, examination dates, fee details, school timings, announcements, homework, transport information, and Parent-Teacher Meeting schedules. This can lead to delays, repeated phone calls, and additional workload for school staff.

ParentConnect AI aims to solve this problem by providing parents with a simple, interactive, and user-friendly chatbot that can respond to common school-related questions quickly and efficiently.

The chatbot is developed using Google Dialogflow, which allows it to understand different ways of asking the same question through intents, entities, parameters, and conversational responses.

🎯 Project Objective
The main objective of ParentConnect AI is to create an efficient communication bridge between parents and the school. 
The chatbot is designed to:

Provide quick access to school information.
Reduce unnecessary manual follow-ups with school staff.
Help parents find important information through a conversational interface.
Improve communication and transparency between parents and the school.
Provide clear and easy-to-understand responses.
Create a more convenient way for parents to interact with school services.
The project follows the requirements of the ParentConnect AI scenario, which focuses on providing information about student attendance, exam schedules, fee details, school announcements, and general school queries.
👨‍👩‍👧 Target Users
The primary users of ParentConnect AI are:
Parents – to access student and school information.
School Staff – to reduce repetitive information requests.
Teachers – to support communication with parents.
💡 Problem Statement
Parents frequently need information from schools, but accessing this information may require phone calls, emails, visits to the school office, or waiting for a response from staff.
Some common problems include:

Difficulty checking attendance.
Forgetting examination dates.
Difficulty accessing fee information.
Missing important school announcements.
Not knowing school timings or holiday dates.
Difficulty getting homework or assignment information.
Repeated questions being asked to school staff.
Delays in receiving basic school information.
ParentConnect AI provides a centralized conversational solution to these problems.
🤖 Main Features
1. Student Attendance
Parents can ask the chatbot about their child's attendance.
Example:

"What is my child's attendance?"
The chatbot can provide information such as attendance percentage, present days, and absent days.
2. Examination Schedule
Parents can ask about upcoming examinations and examination schedules.
Example:

"When are the final exams?"
The chatbot provides the relevant examination information.
3. Fee Information
Parents can ask about school fees and their payment status.
Example:

"Can you show my fee details?"
The chatbot can provide information about fee details and due dates.
4. Fee Payment
The chatbot can guide parents regarding available fee payment methods.
Example:

"How can I pay the school fees?"
5. School Timings
Parents can quickly find school and office timings.
Example:

"What are the school timings?"
6. Holiday Information
Parents can ask about upcoming holidays and the holiday calendar.
Example:

"Show me the holiday list for August."
7. School Announcements
The chatbot can provide important school announcements and updates.
Example:

"Are there any new school announcements?"
8. Parent-Teacher Meeting
Parents can ask about PTM dates and schedules.
Example:

"When is the next Parent-Teacher Meeting?"
9. Homework Information
Parents can ask about their child's homework and assignments.
Example:

"What is today's homework for Grade 8?"
10. School Transport
The chatbot can provide information about school buses, routes, and timings.
Example:

"What is the bus timing for Route 5?"
11. Admission Information
Parents can ask about the admission process.
Example:

"How can I apply for admission?"
12. School Contact Information
The chatbot can provide relevant school contact information.
Example:

"What is the school's contact number?"
🧠 Dialogflow Implementation
ParentConnect AI uses Google Dialogflow to understand natural-language questions from users.
The project includes 15 intents and 10 custom entities, as required by the project brief.

Intents
Welcome Intent
Attendance Intent
Exam Schedule Intent
Fee Details Intent
Fee Payment Intent
School Timings Intent
Holiday Intent
School Announcement Intent
Parent-Teacher Meeting Intent
Homework Intent
Transport Intent
Admission Intent
Contact School Intent
Goodbye Intent
Default Fallback Intent
Each intent contains multiple training phrases so that the chatbot can recognize different ways a parent might ask the same question.
🏷️ Entities
The chatbot uses entities to identify important information from user messages.
The main custom entities include:

@student_name
@grade
@section
@exam_type
@fee_type
@month
@announcement_type
@transport_route
@teacher_name
@department
These entities help the chatbot understand specific information provided by the parent.
For example:

"Show the exam schedule for Grade 8."
Here, Grade 8 can be identified using the @grade entity.
💬 Parameters and Prompts
ParentConnect AI also uses parameters to collect information required to answer certain questions.
For example, if a parent asks:

"What is my child's attendance?"
The chatbot can ask:
"Please enter your child's full name."
It can then ask:
"Please enter your child's grade."
After receiving the required information, the chatbot provides the appropriate response.
This creates a more natural conversational flow instead of requiring the parent to provide all information in one message.

The assignment specifically requires contextual responses, suggestion prompts, and parameter/slot-filling functionality where appropriate.

🔄 Example Conversation
Parent: Hi
ParentConnect AI:
👋 Welcome to ParentConnect AI!

I can help you with:

📊 Attendance
📅 Exam Schedule
💰 Fee Details
📢 Announcements
🚌 Transport
How can I help you?
Parent: What is my child's attendance?

Bot:
Please enter your child's full name.

Parent: Aarav Patel

Bot:
Please enter your child's grade.

Parent: Grade 8

Bot:
📊 Attendance Report

Student: Aarav Patel
Grade: 8
Attendance: 92%
Present: 165 days
Absent: 14 days

Would you like to check anything else?

🧪 Testing and Optimization
The chatbot is tested using different realistic parent queries to ensure that each intent is correctly recognized.
Testing includes:

Testing different ways of asking the same question.
Checking whether the correct intent is triggered.
Checking parameter collection.
Checking whether responses are relevant.
Testing unsupported questions.
Improving training phrases when the chatbot incorrectly identifies an intent.
Testing complete user journeys from beginning to end.
The assignment requires testing with multiple realistic user scenarios and improving the chatbot based on errors or incorrect classifications.
❌ Fallback Handling
If a parent asks a question that ParentConnect AI does not understand, the chatbot provides a friendly fallback response instead of giving an unrelated answer.
Example:

"Sorry, I didn't understand your request. Please ask me about attendance, exams, fees, announcements, transport, or other school services."
This helps maintain a smooth user experience.
🌟 Benefits
ParentConnect AI provides several benefits:
For Parents
Quick access to school information.
Easy conversational interface.
Less waiting for responses.
Convenient access to frequently requested information.
For Schools
Reduces repetitive queries.
Saves administrative time.
Improves communication efficiency.
Provides a centralized communication system.
For Students
Parents can stay updated about attendance, exams, homework, and school announcements.
🚀 Future Improvements
In the future, ParentConnect AI could be expanded with:
Student ID-based authentication.
Real-time database integration.
Firebase/Firestore integration.
Real-time attendance updates.
Online fee payment integration.
Personalized student dashboards.
Multiple-language support.
Voice-based interaction.
Automatic notifications for important announcements.
Integration with the school's existing management system.
These improvements could make the chatbot more suitable for real-world school deployment.
🛠️ Technologies Used
Google Dialogflow
Conversational AI
Natural Language Processing (NLP)
Intents
Entities
Parameters
Slot Filling
Suggestion Prompts
Contextual Responses
📂 Project Structure
ParentConnect-AI/
│
├── README.md
├── Dialogflow/
│   ├── Intents/
│   ├── Entities/
│   └── Responses/
│
├── Documentation/
│   ├── Project_Report.pdf
│   └── Testing_Evidence.pdf
│
└── Screenshots/
    ├── Welcome.png
    ├── Attendance.png
    ├── Exam_Schedule.png
    ├── Fee_Details.png
    └── Announcements.png
📌 Conclusion
ParentConnect AI demonstrates how artificial intelligence and conversational interfaces can be used to solve a practical communication problem in education.
By providing parents with quick access to attendance, examinations, fees, announcements, homework, transport, and other school information, the chatbot can make communication more efficient and user-friendly.

The project demonstrates the practical application of AI, Natural Language Processing, Dialogflow intents, entities, parameters, contextual conversations, and chatbot testing in a real-world school environment.

The overall goal of ParentConnect AI is to create a simple, reliable, and accessible communication bridge between parents and schools.
You can Access CHAT Bot LINk - https://console.dialogflow.com/api-client/demo/embedded/47fc1dce-fd1c-40ab-ac3e-f023e8ff405f
