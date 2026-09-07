# 📊 Habit Impact Lab — Productivity Impact Simulator

Habit Impact Lab is an interactive web-based productivity simulation system that demonstrates how everyday lifestyle habits can influence a user's overall productivity score.

The project uses computational thinking, rule-based scoring, and interactive data visualization to transform daily habit inputs into a measurable Productivity Score.

Users can enter values for study, sleep, screen time, outdoor activity, reading, and exercise. The system evaluates these inputs against predefined healthy or target ranges and generates a productivity score along with personalized improvement feedback.


🌐 Habit Impact Lab — Live Simulator:
https://nailahabib-2005.github.io/Habit-Impact-Lab/

## 📌 Project Overview

Daily habits can have a significant influence on focus, energy, learning, and productivity.

However, it is often difficult for users to understand the combined effect of several habits at the same time.

Habit Impact Lab addresses this idea through a simple interactive simulation.

Instead of presenting separate recommendations for each habit, the system:

1. Collects daily habit information.
2. Evaluates each habit against a target range.
3. Calculates an individual score for each habit.
4. Combines the individual scores.
5. Produces an overall Productivity Score.
6. Provides improvement suggestions.
7. Displays the results through a visual bar chart.

---

## 🎯 Problem Statement

Many students and learners struggle to understand how their daily routines affect their productivity.

Factors such as:

* Study time
* Sleep
* Screen usage
* Outdoor activity
* Reading
* Exercise

can interact with each other and influence daily performance.

Habit Impact Lab provides a simplified computational model that converts these lifestyle inputs into a measurable score.

The purpose is not to predict actual human performance, but to provide an educational and interactive demonstration of how different variables can be evaluated using computational logic.

---

## 💡 Main Concept

The system follows a simple:

```text
Input
  ↓
Habit Evaluation
  ↓
Individual Habit Scores
  ↓
Overall Productivity Score
  ↓
Feedback
  ↓
Visual Graph
```

This makes the project a practical example of:

* Computational thinking
* Rule-based decision making
* Input processing
* Conditional logic
* Data visualization
* User feedback systems

---

## 📝 Input Variables

The application accepts six main lifestyle variables.

| Variable         | Description                    |
| ---------------- | ------------------------------ |
| Study Hours      | Daily time spent studying      |
| Sleep Hours      | Daily sleeping duration        |
| Screen Time      | Daily screen usage             |
| Outdoor Activity | Time spent in outdoor activity |
| Reading Time     | Daily reading duration         |
| Exercise Time    | Daily exercise duration        |

---

## 🧠 Productivity Model

Each input is evaluated against a predefined target range.

The current implementation uses the following ranges:

| Habit            | Target Range |
| ---------------- | -----------: |
| Study            |    2–4 hours |
| Sleep            |    7–9 hours |
| Screen Time      |    3–4 hours |
| Outdoor Activity |      2 hours |
| Reading          |    1–2 hours |
| Exercise         |    1–3 hours |

The system uses a range-based scoring function to calculate how closely each user's input matches the target range.

---

## ⚙️ Scoring Logic

The application calculates an individual score for each habit.

Conceptually:

```text
Habit Input
     ↓
Compare with Target Range
     ↓
Calculate Habit Score
     ↓
Combine Scores
```

If an input falls within its target range, it receives the highest score.

If it falls outside the target range, the score decreases according to its distance from the desired range.

The implemented scoring function ensures that the resulting individual score remains between:

```text
0 – 100
```

---

## 🧮 Overall Productivity Score

The current implementation calculates the final Productivity Score by averaging the six individual habit scores.

Conceptually:

```text
Final Score =
(
Study Score
+
Sleep Score
+
Screen Score
+
Outdoor Score
+
Reading Score
+
Exercise Score
) / 6
```

The final result is rounded to a whole percentage.

Example:

```text
Study Score     = 80
Sleep Score     = 100
Screen Score    = 70
Outdoor Score   = 100
Reading Score   = 90
Exercise Score  = 80

Final Score = Average of all six scores
```

---

## 📊 Score Interpretation

The project can be interpreted using the following general productivity levels:

| Score   | Interpretation        |
| ------- | --------------------- |
| 0–40%   | Low Productivity      |
| 41–70%  | Moderate Productivity |
| 71–100% | High Productivity     |

These categories are intended for simulation and educational purposes.

---

## 🔄 Real-Time Calculation

The system processes the user's inputs when the calculation function is triggered.

The application reads:

```text
Study
Sleep
Screen
Outdoor
Reading
Exercise
```

It then calculates the corresponding scores and updates the Productivity Score displayed on the page.

---

## 💬 Improvement Analysis

One of the main features of Habit Impact Lab is its feedback system.

After calculating the score, the application evaluates each habit separately and generates improvement suggestions.

Examples include:

### Study

If study time is below the target:

> Increase study time toward the recommended target range.

If study time is within the target range:

> Study is in the optimal range.

---

### Sleep

If sleep is below the target:

> Increase sleep toward the 7–9 hour range.

If sleep is within the target range:

> Sleep is optimal.

---

### Screen Time

If screen time is above the target:

> High screen time may increase distraction.

If screen usage is within the target range:

> Screen time is balanced.

---

### Outdoor Activity

If outdoor activity is low:

> Increase outdoor activity for better energy and focus.

---

### Reading

If reading time is low:

> Increase reading time toward the target range.

---

### Exercise

If exercise is low:

> Increase exercise to support energy and mental performance.

---

## 📈 Data Visualization

The project includes a bar chart to visually represent the individual habit scores.

The chart displays:

```text
Study
Sleep
Screen
Outdoor
Reading
Exercise
```

Each category is represented by its corresponding calculated score.

This allows users to quickly identify which habits are performing well and which areas may need improvement.

---

## ⭐ Key Features

### 1. Interactive Inputs

Users can enter their daily lifestyle values.

### 2. Automatic Scoring

The system automatically evaluates the entered values.

### 3. Productivity Score

A final percentage score is generated.

### 4. Habit-Level Analysis

Each lifestyle factor receives its own score.

### 5. Improvement Suggestions

The system provides feedback according to the entered values.

### 6. Visual Representation

A bar chart displays the calculated habit scores.

### 7. Simple User Interface

The application is designed as a lightweight browser-based tool.

---

## 🛠️ Technologies Used

### Frontend

* HTML5
* CSS3
* JavaScript

### Visualization

* Chart.js

### Development

* Visual Studio Code
* Web Browser
* Git
* GitHub

---

## 🧩 Core JavaScript Concepts Demonstrated

The project demonstrates several JavaScript concepts, including:

* DOM manipulation
* User input handling
* Number conversion
* Functions
* Conditional statements
* Mathematical calculations
* Dynamic HTML generation
* Chart rendering
* Data processing

---

## 🔍 Example Scoring Function

The application uses a range-based scoring approach.

Conceptually:

```javascript
function scoreRange(value, min, max) {
    // Evaluate the input against
    // the desired range
    // and return a score between 0 and 100
}
```

This allows different lifestyle variables to be evaluated using the same basic scoring mechanism.

---

## 📊 Visualization Workflow

The chart is generated after the score calculation.

The system passes the individual scores to the chart:

```text
Study Score
Sleep Score
Screen Score
Outdoor Score
Reading Score
Exercise Score
```

The chart then presents these values visually.

---

## 🖥️ How to Run

No server or backend is required.

### Option 1 — Open Directly

Download or clone the repository and open:

```text
Habit-Impact-lab.html
```

in a modern web browser.

---

### Option 2 — VS Code

Open the project in Visual Studio Code and launch the HTML file using a browser or a Live Server extension.

---

## 📂 Project Structure

The current project can be kept as a lightweight single-page application:

```text
habit-impact-lab/
│
├── Habit-Impact-lab.html
└── README.md
```

If the project is later separated into multiple files, the structure can become:

```text
habit-impact-lab/
│
├── index.html
├── style.css
├── script.js
├── assets/
└── README.md
```

---

## 📸 Screenshots

Add screenshots of the actual application here.

Recommended screenshots:

### 1. Main Interface

*Add screenshot here*

### 2. Habit Input Section

*Add screenshot here*

### 3. Productivity Score

*Add screenshot here*

### 4. Improvement Analysis

*Add screenshot here*

### 5. Productivity Graph

*Add screenshot here*

---

## 🌐 Live Demo

Once GitHub Pages is enabled, add the live website here:

```text
https://nailahabib-2005.github.io/habit-impact-lab/
```

---

## 🎓 Educational Purpose

Habit Impact Lab is primarily an educational simulation.

It demonstrates how real-world behavioral variables can be represented computationally using:

* Input variables
* Rules
* Mathematical scoring
* Conditional decision-making
* Feedback
* Visualization

The score should not be interpreted as a scientific, psychological, or medical measurement of an individual's actual productivity.

---

## ⚠️ Limitations

The model is intentionally simplified.

It does not account for many real-world factors such as:

* Individual differences
* Mental health
* Stress
* Work environment
* Academic difficulty
* Sleep quality
* Social circumstances
* Physical health
* Motivation
* Type of study
* Quality of exercise
* Quality of reading

The same target ranges are also not necessarily appropriate for every individual.

Therefore, the generated score should be considered a simulation rather than a clinical or scientific assessment.

---

## 🔮 Future Improvements

Possible future improvements include:

* User accounts
* Daily habit history
* Weekly productivity reports
* Monthly progress tracking
* Local storage
* Firebase integration
* Personalized scoring
* Multiple scoring models
* Improved data visualization
* Habit trend analysis
* Exportable reports
* Dark mode
* Mobile-responsive improvements
* More customizable habit categories

---

## 🚀 Learning Outcomes

This project demonstrates practical understanding of:

* Web development
* JavaScript programming
* Computational thinking
* Decision-making logic
* Data visualization
* User interaction
* Mathematical modeling
* Frontend development

---

## 👩‍💻 Developer

**Naila Habib**

Computer Science | Software Development

GitHub:

```text
https://github.com/nailahabib-2005
```

---

## 📜 License

This project was created for academic, educational, and portfolio purposes.
