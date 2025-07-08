# 🏠 Housing Price Analysis — Hypothesis Testing

This notebook analyzes housing sale prices using hypothesis testing to identify significant differences in mean prices across neighborhoods.

## 📁 Dataset
- **File**: `properties.csv`
- **Source**: Ames Housing Dataset (Kaggle)
- **Focus**: Compare `SalePrice` and determine if neighborhood impacts price.

## 📊 Goals

1. Assess normality of `SalePrice` using:
   - Shapiro-Wilk Test
   - Histogram & KDE
   - Q-Q Plot
   - Skewness & Kurtosis
2. Apply **log transformation** to correct skewness.
3. Conduct independent **t-tests** between neighborhoods:
   - Standard t-test (equal variances)
   - Welch’s t-test (unequal variances)
4. Visualize:
   - Histogram comparisons
   - Violin plots with means
   - Confidence intervals

## 🔬 Key Findings

- Raw sale prices are **right-skewed** and **not normally distributed**.
- Log transformation brings distribution closer to normal.
- Statistically significant difference found in log sale prices between **NAmes** and **CollgCr**.
- Non-overlapping confidence intervals support hypothesis test results.

## 🛠 Requirements

```bash
pip install numpy pandas scipy seaborn matplotlib
