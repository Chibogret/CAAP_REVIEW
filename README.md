# CAAP Mock Exam by Chippo

![Project Logo](logo.png)

## Project Description

This project is a web-based quiz application designed to help users prepare for CAAP (Civil Aviation Authority of the Philippines) mock exams. It is built using HTML, CSS, and vanilla JavaScript, running entirely in the browser.

## Features

*   **Subject Selection:** Users can choose from various aviation-related subjects.
*   **Multiple-Choice Questions:** Presents questions with several options.
*   **Answer Submission & Feedback:** Allows users to submit their answers and receive immediate feedback (correct/incorrect).
*   **Question Skipping:** Users can skip a limited number of questions to attempt later.
*   **Score Tracking:** Dynamically updates and displays the user's score.
*   **Quiz Completion Summary:** Shows a final score and summary at the end of the quiz.
*   **Responsive Design:** Adapts to different screen sizes for usability on various devices.
*   **Client-Side Operation:** Runs entirely in the web browser with no server-side backend required.

## Project Structure

*   `index.html`: The main HTML file that contains the structure, styling (CSS), and JavaScript logic for the quiz application.
*   `logo.png`: The project's logo image displayed on the splash screen and in this README.
*   `*.json` (e.g., `Air Law.json`, `Meteorology.json`, `questions.json`): These JSON files store the quiz questions, options, and correct answers for each subject. Each file typically represents a different exam topic.

## Quiz Data Format

The quiz questions are stored in JSON files (e.g., `Air Law.json`). Each file follows this structure:

```json
{
    "exam_title": "Name of the Exam or Subject",
    "questions": [
        {
            "question_number": 1,
            "question_text": "What is the question?",
            "options": [
                "Option A",
                "Option B",
                "Option C",
                "Option D"
            ],
            "correct_answer": "Option B"
        },
        {
            "question_number": 2,
            "question_text": "Another question...",
            "options": ["True", "False"],
            "correct_answer": "True"
        }
        // ... more questions
    ]
}
```

*   `exam_title`: A string representing the title of the quiz or subject.
*   `questions`: An array of question objects.
    *   Each question object contains:
        *   `question_number`: An integer identifier for the question.
        *   `question_text`: A string containing the actual question.
        *   `options`: An array of strings representing the choices for the question.
        *   `correct_answer`: A string that must exactly match one of the items in the `options` array.

## How to Use / Setup

This quiz application is designed to run directly in your web browser. No complex setup or server is required.

1.  **Clone or Download:** Get a copy of the project files.
2.  **Open `index.html`:** Navigate to the project directory and open the `index.html` file in any modern web browser (e.g., Chrome, Firefox, Edge, Safari).
3.  **Select a Subject:** Use the dropdown menu to choose the quiz subject you want to practice.
4.  **Start Quiz:** The first question will be displayed, and you can begin the quiz.

## Future Enhancements

While this application is fully functional for its purpose, here are some potential ideas for future improvements:

*   **Add More Subjects:** Expand the question bank with more JSON files for other subjects.
*   **Enhanced UI/UX:** Improve the visual design and user experience with more interactive elements or animations.
*   **Question Randomization:** Implement more sophisticated randomization for the order of questions and options.
*   **Persistent Scores:** Allow users to save their scores (e.g., using browser local storage).
*   **Review Incorrect Answers:** Add a feature to review questions that were answered incorrectly.
*   **Timer:** Implement a timer for each question or for the overall quiz.
*   **PWA (Progressive Web App):** Convert the application into a PWA for offline access and app-like features.
