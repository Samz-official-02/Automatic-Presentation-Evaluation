# Automatic Presentation Evaluation System

## Overview

**The Automatic Presentation Evaluation System is a web application designed to evaluate student presentations based on video and audio inputs. It provides features for user registration, login, student management, and detailed analysis of presentation videos. The system uses various deep learning models and APIs to process video and audio data, providing feedback on different aspects of the presentation such as emotions, speech rate, and sentiment.**

# Business Use Case

## Problem Statement:

Many educational institutions struggle with the objective and efficient evaluation of student presentations. Traditional methods of assessment are often time-consuming and subject to human biases. Additionally, providing detailed feedback on multiple aspects such as emotions, speech rate, and sentiment can be challenging for educators, especially when dealing with large classes.

## Business Use Case:

An educational institution wants to implement a solution that can automatically evaluate student presentations, ensuring consistency, fairness, and detailed feedback. This solution should save time for educators and provide valuable insights to help students improve their presentation skills.

## Solution:

The Automatic Presentation Evaluation System addresses these challenges by leveraging advanced machine learning and deep learning techniques to analyze video and audio data from student presentations. By automating the evaluation process, the system provides detailed, objective feedback on various aspects of the presentation.

## How This System Solves the Problem:

1. Objective Evaluation: The system uses pre-trained ONNX models to analyze emotions and various Python libraries along with the Deepgram API to evaluate speech sentiment and rate. This ensures that the evaluation is consistent and free from human biases.

2. Detailed Feedback: The system generates comprehensive PDF reports for each presentation, highlighting strengths and areas for improvement in aspects such as emotion, speech rate, and sentiment. This detailed feedback is valuable for students to understand and improve their presentation skills.

3. Time Efficiency: Automating the evaluation process saves significant time for educators, allowing them to focus on other important tasks. The system can process and evaluate multiple presentations quickly and accurately.

4. Scalability: The system can handle large volumes of presentations, making it suitable for institutions with a large number of students. The backend infrastructure, including MongoDB and GridFS, ensures efficient data storage and retrieval.

5. Enhanced Learning Experience: By providing objective and detailed feedback, the system enhances the learning experience for students. They receive actionable insights that help them refine their presentation skills, contributing to their overall academic development.

## Implementation in an Educational Institution:

1. **Setup:** The institution deploys the Automatic Presentation Evaluation System on the cloud or local servers, ensuring secure access for educators and students.

2. **User Management:** Educators and students register on the platform. Educators manage student details and oversee the evaluation process.

3. **Presentation Upload:** Students upload their presentation videos through the user-friendly dashboard. The system processes these videos to analyze various parameters.

4. **Evaluation and Feedback:** The system generates detailed reports for each presentation, which are reviewed by educators and shared with students. Educators can use the dashboard to track progress and manage evaluations.

5. **Continuous Improvement:** The feedback provided by the system helps students continuously improve their presentation skills. Educators can also use the data to identify common areas of improvement and tailor their teaching methods accordingly.

By implementing the Automatic Presentation Evaluation System, educational institutions can enhance the efficiency, objectivity, and quality of their student presentation evaluations, ultimately contributing to better learning outcomes.


## Cloud Deployment Link

[Automatic Presentation Evaluation](https://automatic-presentation-evaluation.onrender.com)


## Features

* **User Registration and Login:** Secure user registration and login functionality using hashed passwords.
* **Student Management:** Register and manage student details.
* **Video Processing:** Upload and process presentation videos to analyze emotions using a pre-trained ONNX model.
* **Audio Processing:** Extract and analyze audio from videos to evaluate speech sentiment, rate, and other parameters using Deepgram API and various Python libraries.
* **PDF Report Generation:** Generate detailed PDF reports for each student presentation evaluation.
* **Dashboard:** User dashboard to view and manage evaluations.
* **Session Management:** Secure session management for logged-in users.

## Technologies Used

* **Backend:** Flask, MongoDB, GridFS, threading
* **Frontend:** HTML, CSS, JavaScript
* **Machine Learning:** OpenCV, ONNX, VaderSentiment, TextBlob, librosa
* **APIs:** Deepgram API for speech-to-text transcription


## Installation

1. **Clone the repository:**

```
git clone https://github.com/your-username/presentation-evaluation-system.git
cd presentation-evaluation-system
```

2. **Install required dependencies:**

```
pip install -r requirements.txt
```

3. **Set up MongoDB:**

* Create a MongoDB Atlas cluster or use a local MongoDB instance.
* Update the MongoDB connection URI in `app.py`

```
uri = "your-mongodb-connection-uri"
```

4. **Set up Deepgram API:**

* Sign up for a Deepgram account and get your API key.
* Update the API key in `Speech_Sentiment_Analyzer.py`:

```
api_key = "your-deepgram-api-key"
```


5. **Run the application:**

```
python application.py
```

6. **Access the application:**

Open your web browser and navigate to `http://0.0.0.0:8000`.


## Usage

1. **User Registration and Login:**
   * Register as a new user or login with existing credentials.
2. **Student Management:**
   * Register new students with details like name, class, section, roll number, and gender.
3. **Video Upload and Processing:**
   * Upload presentation videos through the dashboard.
   * The system will process the video to analyze emotions and extract audio for further analysis.
4. **View Results and Download Reports:**
   * View the evaluation results on the dashboard.
   * Download detailed PDF reports for each presentation.



## License

This project is licensed under the MIT License. See the `LICENSE` file for details.


## Acknowledgements

* [Deepgram API](https://www.deepgram.com/)
* [VaderSentiment](https://github.com/cjhutto/vaderSentiment)
* [TextBlob](https://textblob.readthedocs.io/en/dev/)
* [Librosa](https://librosa.org/)
* [OpenCV](https://opencv.org/)
* [ONNX](https://onnx.ai/)


**Feel free to contact me if you have any questions or need further assistance. Happy coding!**
