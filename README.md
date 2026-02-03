# Assignment-1: Learning Probability Density Function using NO₂ Data

## Objective
To learn the parameters of a probability density function (PDF) by applying a roll-number-dependent non-linear transformation on NO₂ air quality data and estimating the distribution using statistical techniques.

---

## Learning Resource
• India Air Quality Dataset (Kaggle)  
• Concepts of Probability Density Functions  
• Maximum Likelihood Estimation (MLE)

---

## In this assignment we learn

• **Getting Data:**  
  How to load real-world air quality data and select NO₂ as the feature.

• **Data Cleaning:**  
  How to handle missing values before statistical modeling.

• **Feature Transformation:**  
  How to apply a roll-number-parameterized non-linear transformation  
  \( z = x + a_r \sin(b_r x) \)

• **Statistical Modeling:**  
  How to model transformed data using a Gaussian-shaped probability density function.

• **Parameter Estimation:**  
  How to estimate μ and σ² using Maximum Likelihood Estimation (MLE).

• **Model Parameter Computation:**  
  How to compute λ and normalization constant c for a valid PDF.

• **Predicted Probability Density:**  
  How to compute the predicted probability density \( \hat{p}(z) \) for each data point.

• **Model Validation:**  
  Understanding normalization and interpretation of probability density values.

• **Result Interpretation:**  
  How learned parameters describe the distribution of transformed NO₂ values.


## Tools Used
- Python
- NumPy
- Pandas

---

## Conclusion
This implementation shows how a non-linear transformation and maximum likelihood estimation can be used to learn a valid and normalized probability density function for real-world air quality data.


