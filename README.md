## Project: Personalized Quiz Analysis and Recommendations

### Overview
This project analyzes quiz performance data to generate personalized insights and recommendations for a user. The analysis combines:
1. **Current Quiz Data**: Details of a user's latest quiz submission (topics, responses, and performance).
2. **Historical Quiz Data**: Performance data from the last 5 quizzes for each user.

### Files
The project uses three key input files:
- **Api_endpoint.json**: Contains historical quiz performance data.
- **Quiz_submission_data.json**: Contains details about the latest quiz submission for a specific user.
- **Quiz_endpoint.json**: Metadata about quizzes, including topics, structure, and scoring.

### Steps in the Analysis
#### 1. **Load and Preprocess Data**
- Read JSON files and normalize nested data into pandas DataFrames.
- Merge current quiz data (`submission_df` and `quiz_df`) and historical data (`api_df`).

#### 2. **Analyze Current Quiz Data**
- Extract key metrics, including:
  - **Score**: Total score achieved in the latest quiz.
  - **Accuracy**: Percentage of correct answers.
  - **Speed**: User's response speed.
  - **Mistakes**: Number of mistakes relative to the maximum allowed.
  - **Topic**: The topic of the quiz.

#### 3. **Analyze Historical Quiz Data**
- Compare the user's current performance to their historical averages (if available).
- Calculate trends in score, accuracy, and speed across previous quizzes.

#### 4. **Generate Insights**
- Identify strengths and weaknesses in the user's performance.
- Highlight issues such as low accuracy, slow speed, or exceeding allowed mistakes.

#### 5. **Provide Recommendations**
- Suggest areas of focus for improvement (e.g., reviewing mistakes, practicing timed quizzes).
- Highlight topics where the user can improve.

#### 6. **Visualization**
- Generate a bar chart summarizing the user's performance in the current quiz.

### Code Structure
The analysis is structured into blocks for use in a Jupyter Notebook:
1. **Import Libraries**: Load required libraries.
2. **Load and Preprocess Data**: Read and clean input data.
3. **Analyze Current Quiz**: Extract metrics and insights from the latest quiz.
4. **Analyze Historical Data**: Compare current performance to historical trends.
5. **Generate Insights and Recommendations**: Provide actionable suggestions based on analysis.
6. **Visualization**: Create visual summaries of user performance.

### How to Run
1. Clone the repository:
   ```bash
   git clone <https://github.com/sidkhatod/testline_task>
   cd <testline_task>
   ```

2. Install dependencies:
   ```bash
   pip install pandas matplotlib seaborn
   ```

3. Place the input JSON files in the project directory.

4. Run the Jupyter Notebook:
   ```bash
   jupyter notebook testline.ipynb
   ```

5. Follow the blocks in the notebook to process the data, generate insights, and visualize results.

### Outputs
- **Insights**: Key observations about the user's performance in the latest quiz.
- **Recommendations**: Tailored suggestions to help the user improve.
- **Visualization**: A bar chart summarizing performance metrics.

### Example Insights and Recommendations
#### Insights:
- "Accuracy is below 90%. Focus on reviewing mistakes to improve."
- "Mistakes made exceeded the allowed limit."

#### Recommendations:
- "Review incorrect answers from this quiz to avoid repeated mistakes."
- "Practice with timed quizzes to improve response speed."

### Future Improvements
- **Enhanced Trend Analysis**: Include visualizations of historical trends over time.
- **Topic-Specific Insights**: Drill down into performance by subtopics.
- **Scalability**: Extend the analysis to handle data for multiple users at scale.

### Dependencies
- Python 3.7+
- Pandas
- Matplotlib
- Seaborn

---

