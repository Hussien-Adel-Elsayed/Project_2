# Math Quiz Game (C++ Console Application)

Math Quiz Game (C++ Console Application)
This project is a simple, command-line Math Quiz Game built in C++. It's designed to provide a customizable and engaging way to practice basic arithmetic skills (Addition, Subtraction, Multiplication, and Division) across various difficulty levels.

🎯 Game Features and Customization
The game is highly configurable at the start of each session:

Number of Questions: The user determines the total number of questions they wish to answer (up to 10 questions).

Difficulty Levels (enQuestionLevel):

Easy: Numbers between 1 and 10.

Medium: Numbers between 10 and 50.

Hard: Numbers between 50 and 100.

Mix: Randomly selects a difficulty level for each question.

Operation Types (enOperationType):

Add (+)

Subtract (-)

Multiply (*)

Divide (/)

Mix: Randomly selects an operation for each question.

Instant Feedback: The screen color changes immediately after the user answers:

Green: Correct Answer (system("color 2f"))

Red: Wrong Answer (system("color 4f"))

Final Results Summary: At the end of the quiz, a detailed summary is displayed, including:

Overall Pass/Fail status (Pass if correct answers 
≥
 wrong answers).

Question Level and Operation Type used.

Count of Right and Wrong Answers.

🏗️ Code Structure and Logic
The game is structured using modular C++ components for clarity:

Enums: Used extensively (enQuestionLevel, enOperationType) to make choices and logic human-readable, avoiding the use of magic numbers.

Structs for Data:

stQuestion: Holds data for a single math problem (the two numbers, operation, correct answer, player's answer, and result).

stQuizz: Aggregates the entire quiz state (list of questions, total counts, final pass status).

Key Functions:

GenerateQuestion: Logic to create the random numbers and operation based on the selected level and type.

SimpleCalculeto: A core function to calculate the correct answer for any given two numbers and operation type.

AskAndCorrectQuestionListAnswer: Manages the main game loop, displaying the question, reading input, and correcting the answer.

This modular design makes the application easy to maintain and simple to extend if new features are desired, such as adding more complex operations (like exponents or modulus) or new difficulty levels.

🎮 How to Play
Compile and run the C++ application.

Follow the on-screen prompts to configure your quiz:

Enter the desired number of questions.

Select the difficulty level (1 to 4).

Select the operation type (1 to 5).

Answer each math question by typing your answer and pressing Enter.

Observe the instant color feedback.

View your final results summary.

You will be asked if you want to play again.


Count of Right and Wrong Answers.
