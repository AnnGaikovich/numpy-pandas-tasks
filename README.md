# Pandas and Numpy tasks

## Requirements

- **NumPy** – core numeric operations
- **Pandas** – data manipulation
- **SciPy** – only used for `cdist` comparison in the distance matrix task (optional)

## Datasets

- **`cereal.csv`** – a column of calorie values for various breakfast cereals.  
  (One column, no header, used for the CrunchieMunchies marketing analysis.)

- **`adult.data.csv`** – the classic UCI Adult Census Income dataset.  
  Features include age, workclass, education, marital status, occupation, race, sex, capital gain/loss, hours per week, native country, and salary (>50K / ≤50K).

Place both files inside a `data/` folder in the root of the repository.


## Exercises Overview

### `assignment_numpy.ipynb`

| Section | Description |
|---------|-------------|
| Basic tasks (1‑6) | Element‑wise operations, max replacement, Cartesian product, row filtering, removing duplicates |
| Problem 1 | Product of non‑zero diagonal elements (pure Python vs vectorized) |
| Problem 2 | Check if two vectors represent the same multiset |
| Problem 3 | Max element immediately after a zero |
| Problem 4 | Run‑length encoding (two implementations) |
| Problem 5 | Pairwise Euclidean distance matrix + comparison with `scipy.spatial.distance.cdist` |
| Problem 6 | **CrunchieMunchies analysis** – load cereal calories, compute mean, median, percentiles, percentage above 60 kcal, standard deviation, and generate a marketing insight paragraph |

### `assignment_pandas.ipynb`

| Task | Description |
|------|-------------|
| 1 | Count of males / females |
| 2 | Mean age of males |
| 3 | Proportion of US citizens |
| 4‑5 | Mean and standard deviation of age per salary group |
| 6 | Verify if all high‑income individuals have at least a bachelor’s degree |
| 7 | Age statistics by race and sex; find max age of Asian‑Pacific‑Islander males |
| 8 | Compare high‑income proportion between married and unmarried men |
| 9 | Maximum hours per week, count of such people, and their rich‑percentage |
| 10 | Mean working hours per country and salary level |
| 11 | Create `AgeGroup` column (young / adult / retiree) |
| 12‑13 | Count >50K per age group and identify the group with the highest proportion |
| 14 | Filter occupation groups where mean age ≤ 40 and min hours > 5 |

All tasks are implemented using clean, vectorised Pandas operations.

## Output

- The notebooks print results directly.
- For the CrunchieMunchies task, a summary paragraph is printed.
- Optionally, you can save any DataFrame to `output/` (e.g., `data.to_csv('output/result.csv')`).
