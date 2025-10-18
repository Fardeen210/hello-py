# Improve Regression Performance via Feature Engineering

You are given the dataset: `task/data/movies.csv`.

**Goal:**  
Train a simple regression model (e.g., LinearRegression or RandomForestRegressor or any suitable model)  
to predict a **numeric target column** in the dataset.

Your objective is to **improve model performance (R² score)** over the baseline
by performing basic feature engineering (e.g., selecting, scaling, encoding, or
transforming features).

---
## Final Step
When you finish your analysis, you must call the `submit_answer` tool
with your final JSON answer.

The answer should include:
- `"r2_score"` — your model's R² score on the test set
- `"baseline_r2"` — R² score from a baseline LinearRegression
- `"features_used"` — list of the columns you used

Example:
{
  "type": "tool_use",
  "name": "submit_answer",
  "input": {
    "answer": {
      "r2_score": 0.84,
      "baseline_r2": 0.76,
      "features_used": ["YEAR_numeric", "VOTES_numeric", "GENRE_count"]
    }
  }
}