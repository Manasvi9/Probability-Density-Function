# Assignment-1: Learning Probability Density Function using NO₂ Data

## Objective
To learn the parameters of a probability density function (PDF) by applying a roll-number-dependent non-linear transformation on NO₂ air quality data and estimating the distribution using statistical techniques.

---

## Dataset
- **Source:** India Air Quality Dataset (Kaggle)
- **File Used:** `city_day.csv`
- **Feature:** `NO2`
- Missing values are removed before processing.

---

## Transformation
Each NO₂ value \( x \) is transformed into \( z \) using:

\[
z = x + a_r \sin(b_r x)
\]

where:
\[
a_r = 0.05 \times (r \bmod 7)
\]
\[
b_r = 0.3 \times (r \bmod 5 + 1)
\]

and \( r \) is the university roll number.

---

## Probability Density Function
The transformed variable \( z \) is modeled using:

\[
\hat{p}(z) = c \cdot e^{-\lambda (z - \mu)^2}
\]

---

## Parameter Estimation
- Mean \( \mu \) and variance \( \sigma^2 \) are estimated using **Maximum Likelihood Estimation (MLE)**.
- Remaining parameters are computed as:

\[
\lambda = \frac{1}{2\sigma^2}
\]
\[
c = \sqrt{\frac{\lambda}{\pi}}
\]

This ensures the PDF is properly normalized.

---

## Learned Parameters
mu = 21.147713187307595
lambda = 0.00229778768143052
c = 0.027044565726790013

---

## Sample Predicted Probability Densities
[0.02608736 0.01683214 0.02408164 0.02468327 0.01735768]

> Note: These values represent **probability density**, not direct probabilities.

---

## Tools Used
- Python
- NumPy
- Pandas

---

## Conclusion
This implementation shows how a non-linear transformation and maximum likelihood estimation can be used to learn a valid and normalized probability density function for real-world air quality data.


