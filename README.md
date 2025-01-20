Personalized Student Recommendations Solution

Project Overview

This project focuses on analyzing quiz performance to provide students with personalized recommendations for improving their preparation. The solution processes historical and current quiz data, identifies performance patterns, and generates actionable insights to help users enhance their learning outcomes.

Key Features:

Data Analysis: Processes quiz performance data to identify trends and patterns by topics, difficulty levels, and accuracy.

Insights Generation: Highlights weak areas, improvement trends, and performance gaps for each user.

Personalized Recommendations: Provides actionable suggestions on topics, question types, and difficulty levels to focus on.

Student Persona Definition: Categorizes users into personas based on their strengths and weaknesses.

Requirements

Dependencies

Install the following Python libraries:

pip install pandas matplotlib seaborn

Data Files

The solution processes the following input files:

API Data: Performance data from the last 5 quizzes for each user.

Quiz Submission Data: Details of a user’s latest quiz submission.

Quiz Metadata: Schema containing topics and metadata for quizzes.

Ensure the data files are placed in the root directory of the project:

api_endpoint.json

quiz_submission_data.json

quiz_endpoint.json

Setup Instructions

Clone the repository:

git clone <repository_url>
cd <repository_name>

Ensure the required data files are in place.

Run the script:

python analyze_quiz_data.py

Approach Description

1. Data Loading and Preprocessing

Load data from JSON files.

Normalize and merge datasets based on user_id and quiz_id.

Clean the merged dataset by renaming columns and removing redundant fields.

2. Data Analysis

Calculate performance metrics such as:

Topic-wise accuracy

Difficulty level trends

Response accuracy and improvement rates

Identify weak areas for each user.

3. Insights Generation

Generate visualizations using matplotlib and seaborn.

Highlight areas requiring improvement and strengths.

4. Personalized Recommendations

Provide actionable steps, such as:

Suggested topics and difficulty levels.

Recommended question types based on past performance.

5. Bonus: Student Persona Definition

Define user personas by clustering performance patterns and labeling them creatively.

Visualizations

Heatmaps for topic-wise performance.

Line plots showing improvement trends.

Bar charts highlighting weak areas.

Demonstration Video

The solution includes a demonstration video:

Duration: 2-5 minutes

Content:

Sample input and output

Explanation of insights and recommendations logic

Screenshots

Include visualizations such as:

Topic-wise performance heatmaps

Weak area identification bar charts

Contribution

Feel free to contribute by submitting a pull request or suggesting enhancements in the issues section.

Contact

For queries, contact [your_email@example.com].

