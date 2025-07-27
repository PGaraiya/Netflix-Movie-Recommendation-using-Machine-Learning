# Netflix Movie Recommendation using Machine Learning

## Overview

This project utilizes the **Apriori algorithm** to discover association rules between movies in a dataset, specifically focusing on movie transactions. By analyzing patterns in users’ watching habits, the project identifies pairs (and potentially groups) of movies that are frequently watched together. These insights are then used to provide movie recommendations to users,enhancing the Netflix experience by surfacing relevant content based on historical data.

## Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Dataset

The dataset consists of movie transactions, where each transaction represents a set of movies watched together by a user. Commonly, this dataset is formatted so that each row corresponds to a single viewing session, with movies separated by commas.

Example:
```
Movie1, Movie2, Movie3
Movie2, Movie4
Movie1, Movie4, Movie5
```

> **Note:** You can use your own movie transaction dataset or sample data provided in the repository.

## Features

- **Data Preprocessing:** Cleans and structures the movie transaction data for analysis.
- **Apriori Algorithm Implementation:** Finds frequent itemsets and association rules among watched movies.
- **Recommendation Engine:** Suggests movies to users based on identified associations.
- **Google colab** Interactive analysis and visualization for easy experimentation.

## Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/PGaraiya/Netflix-Movie-Recommendation-using-Machine-Learning.git
   cd Netflix-Movie-Recommendation-using-Machine-Learning
   ```

2. **Install required dependencies:**
   - Make sure you have [Python 3.x](https://www.python.org/downloads/) installed.
   - It is recommended to use a virtual environment.

   ```bash
   pip install -r requirements.txt
   ```

   > If `requirements.txt` is not available, the main libraries you’ll need are:
   - `apyori`  ## first install and then import apriori from it
   - `pandas`
   - `matplotlib.pyplot`
   - `numpy`

  

## Usage

1. **Start Jupyter Notebook:**
   ```bash
   Jupyter Notebook
   ```

2. **Open the main Notebook** (`Netflix_Movie_Recommendation.ipynb`) and follow the step-by-step instructions.

3. **Steps covered in the Notebook:**
   - Load and preprocess the dataset
   - Apply Apriori algorithm to discover frequent movie combinations
   - Generate association rules
   - Use rules to make recommendations

## Results

- **Frequent Movie Pairs:** The analysis reveals which movies are commonly watched together, e.g., `"Inception"` and `"Interstellar"`.
- **Association Rules:** If a user watches Movie A, there’s a high likelihood they’ll watch Movie B.
- **Recommendations:** Users can be recommended movies based on their current watching history and discovered associations.

## Contributing

Contributions are welcome! If you have suggestions, bug reports, or improvements, please feel free to open an issue or submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).

## Acknowledgements

- [mlxtend](http://rasbt.github.io/mlxtend/) library for Apriori implementation
- Publicly available movie transaction datasets

---

**Happy Recommending!**
