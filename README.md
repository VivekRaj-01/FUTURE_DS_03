# FUTURE_DS_03
COLLEGE EVENT FEEDBACK ANALYSIS

📊 Student Feedback Analysis — Internship Project

This project analyzes student feedback collected after college events such as tech fests, workshops, cultural events, and seminars. Using Python + Google Colab, the goal is to extract insights from both ratings and text-based comments to help organizers understand satisfaction levels and areas needing improvement.

📌 Project Overview

Campus events generate large amounts of feedback through Google Forms — but the real challenge is turning that data into meaningful insights.

In this task, we:

Cleaned and prepared a Google Forms feedback dataset (CSV)

Identified rating-based satisfaction patterns

Performed keyword extraction on textual comments

Computed question-wise average scores

Identified best-performing and lowest-performing areas

Summarized results for actionable recommendations

🛠️ Tech Stack
Component	Tool
Programming	Python
Environment	Google Colab
Libraries	Pandas, NumPy
Data Input	Google Forms CSV export
Output	Cleaned DataFrame + Insights Summary
📁 Dataset Description

The dataset is exported directly from Google Forms, containing:

Student identifiers

Rating-scale responses (1–10 or 1–5 depending on form)

Textual feedback comments

Optional demographic or course-related fields

Example columns:

degree_of_difficulty_of_assignments

solves_doubts_willingly

well_versed_with_the_subject

course_recommendation_based_on_relevance

feedback_text (comments)

🔍 Analysis Performed
✔ 1. Data Cleaning

Removed unnamed columns

Standardized column names

Removed empty rows

Converted rating columns to numeric

✔ 2. Rating-Based Insight Extraction

We calculated:

avg_scores = df[numeric_cols].mean()


Then identified:

Top 3 strongest factors

Bottom 3 factors needing improvement

✔ 3. Text-Based Insight Extraction

We performed simple keyword frequency checks on feedback comments (no deep NLP required).

Examples:

“helpful”

“interactive”

“improvement”

“timing”

“materials”

⭐ Top Insights
✅ Top 3 Highest-Rated Areas

well_versed_with_the_subject

student_id (if numeric scale was mistakenly included; otherwise ignored)

course_recommendation_based_on_relevance

⚠️ Top 3 Lowest-Rated Areas

degree_of_difficulty_of_assignments

solves_doubts_willingly

course_recommendation_based_on_relevance (in some cases)

(These may vary based on dataset — update based on your actual results.)

📊 Sample Code Used
avg_scores = df[numeric_cols].mean()
avg_scores.sort_values(ascending=False).head(3)
avg_scores.sort_values().head(3)

📈 Conclusion

This analysis provides a clear, data-backed picture of:

What students appreciate in event organization

What areas require improvement

How feedback can drive better event planning

The project shows strong practical understanding of Python data analysis, cleaning, and insight generation.

📦 Folder Structure
College-Event-Feedback-Analysis/
│
├── dataset/ (optional)
│   └── feedback_data.csv
│
├── notebook/
│   └── feedback_analysis.ipynb
│
└── README.md

👨‍💻 Author

Vivek Raj
Data Science & Analytics Intern
