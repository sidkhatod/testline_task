# Personalized Student Recommendations Solution

## Project Overview

This project focuses on analyzing quiz performance to provide students with personalized recommendations for improving their preparation. The solution processes historical and current quiz data, identifies performance patterns, and generates actionable insights to help users enhance their learning outcomes.

## Key Features

- **Data Analysis**: Processes quiz performance data to identify trends and patterns by topics, difficulty levels, and accuracy.
- **Insights Generation**: Highlights weak areas, improvement trends, and performance gaps for each user.
- **Personalized Recommendations**: Provides actionable suggestions on topics, question types, and difficulty levels to focus on.
- **Student Persona Definition**: Categorizes users into personas based on their strengths and weaknesses.

## Requirements

### Dependencies

Install the following Python libraries:

```bash
pip install pandas matplotlib seaborn
```
# Quiz Data Analysis

This repository contains a solution for analyzing user performance across multiple quizzes. The analysis uses historical performance data, current quiz submission data, and quiz metadata to generate insights into user strengths, weaknesses, and overall performance.

## Data Files

The solution processes the following input files:

- **API Data**: Performance data from the last 5 quizzes for each user.
- **Quiz Submission Data**: Details of a user's latest quiz submission.
- **Quiz Metadata**: Schema containing topics and metadata for quizzes.

Ensure the following data files are placed in the root directory of the project:

- `api_endpoint.json`
- `quiz_submission_data.json`
- `quiz_endpoint.json`

## Setup Instructions

### Clone the repository:

```bash
git clone <repository_url>
cd <repository_name>

