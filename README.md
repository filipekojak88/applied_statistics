# Applied Statistics — Assessment Problems (ATU)

This repository contains my submission for the **Applied Statistics** assessment taught by by the lecturer Ian McLoughlin in ATU, delivered in a single Jupyter notebook: `problems.ipynb`, which codes follow PEP 8 conversions. The notebook solves the four required problems using a mix of **analytical reasoning**, **simulation**, and **hypothesis testing**, with explanations and references included throughout. 

This README has been written with [Github's documentation on README](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes) in mind. MarkDown was used in this README file and was based on [GitHub's Documentation](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

## Project Structure

Repository: applied_statistics

| File                 | Description |
|----------------------|-------------|
| `.gitignore`         | Prevents unnecessary or auto-generated files from being committed |
| `README.md`          | Project overview and instructions (this file) |
| `problems.ipynb`     | Full assessment notebook containing all four problems |
| `requirements.txt`   | Python dependencies required to run the notebook |

## Problems covered

The notebook addresses the four assessment problems:

1. **Extending the Lady Tasting Tea**    
This problem extends Fisher’s original Lady Tasting Tea experiment by increasing the design from 8 cups to 12 cups. Using simulation, the probability of correctly identifying all cups by chance is estimated for both designs and compared. The aim is to show how increasing the number of cups strengthens the statistical evidence against random guessing, while keeping the hypothesis-testing framework unchanged.

2. **Normal Distribution**     
This problem investigates sampling variability in estimates of the standard deviation. A large number of samples are drawn from a standard normal distribution, and the standard deviation is computed using both ddof = 0 (population SD) and ddof = 1 (sample SD). By comparing their sampling distributions, the problem illustrates estimator bias, variability, and how these properties change as sample size increases.

3. **t-Tests**     
This problem explores Type II error in hypothesis testing using simulation. Independent samples are drawn from normal distributions with increasing differences in means, and two-sample t-tests are repeatedly performed. The proportion of times the null hypothesis is not rejected is estimated and plotted, demonstrating how the Type II error rate decreases as the true difference between means increases.

4. **ANOVA**
This problem compares one-way ANOVA with multiple pairwise t-tests when analysing more than two group means. Three samples with different population means are generated, and both approaches are applied. The results are compared to show how ANOVA provides a single global test while controlling the overall error rate, highlighting why ANOVA is preferred over running several independent t-tests.

## How to run

### Prerequisites
- **Python 3.10+** (recommended)
- **pip** (Python package installer)
- **Jupyter Lab** or **Jupyter Notebook** (to open and run `.ipynb` files)
- (Optional) **Git** to clone the repository

> Note: All required Python packages are listed in `requirements.txt`.

### Setup Steps

1. **Clone the repository**
   ```bash
   git clone <REPOSITORY_URL>
   cd applied_statistics
   ```

2. **Create a virtual environment (recommended)**    
    This keeps the project dependencies isolated from other Python projects.

    For macOS / Linux
    ```bash
    python3 -m venv .venv
    source .venv/bin/activate        # On Windows(PowerShell): .\.venv\Scripts\Activate.ps1
    ```

3. **Install dependencies**
    ```bash
    pip install -r requirements.txt
    ```

4. **Launch Jupyter**    
    Option A: Jupyter Lab
    ```bash
    jupyter lab
    ```
    Option B: Classic Jupyter Notebook
    ```bash
    jupyter notebook
    ```

5. **Open and run the notebook**

    Open: `problems.ipynb`

    Run all cells from top to bottom (e.g., Kernel → Restart & Run All in most interfaces).

---