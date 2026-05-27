```python
import numpy as np

scores = [88, 92, 79, 85, 95, 81, 86, 90, 83, 77, 89]

# Original mean and standard deviation
mean_orig = np.mean(scores)
std_orig = np.std(scores, ddof=1)

print(f"Original mean: {mean_orig:.4f}")
print(f"Original std: {std_orig:.4f}")

# Remove highest and lowest
scores_sorted = sorted(scores)
scores_filtered = scores_sorted[1:-1]

print(f"Filtered scores: {scores_filtered}")

# New mean and standard deviation
mean_new = np.mean(scores_filtered)
std_new = np.std(scores_filtered, ddof=1)

print(f"New mean: {mean_new:.4f}")
print(f"New std: {std_new:.4f}")


```

```text
Original mean: 85.9091
Original std: 5.5759
Filtered scores: [79, 81, 83, 85, 86, 88, 89, 90, 92]
New mean: 85.8889
New std: 4.3141


```


### **1. Theory: Mean and Standard Deviation**

* **Mean ($\bar{x}$):** The mean is the arithmetic average of a dataset, calculated by summing all the values ($x_i$) and dividing by the total number of values ($N$).

$$\bar{x} = \frac{1}{N} \sum_{i=1}^{N} x_i$$


* **Standard Deviation ($\sigma$):** Standard deviation measures the amount of variation or dispersion in a set of values. A low standard deviation indicates that the values tend to be close to the mean. Because we are looking at a sample of students (and the prompt provides the $N-1$ denominator), we use the **sample standard deviation** formula (Note: the mathematical definition includes taking the square root of the variance):

$$\sigma = \sqrt{\frac{1}{N-1} \sum_{i=1}^{N} (x_i - \bar{x})^2}$$



---

### **2. Determination: Part 1 (Original Scores)**

**Given Data ($N = 11$):**
Scores: 88, 92, 79, 85, 95, 81, 86, 90, 83, 77, 89

**Step A: Calculate the Original Mean**
Sum of all scores: $88 + 92 + 79 + 85 + 95 + 81 + 86 + 90 + 83 + 77 + 89 = 945$


$$\bar{x} = \frac{945}{11}$$

$$\bar{x} \approx 85.91$$

**Step B: Calculate the Original Standard Deviation**
First, subtract the mean from each score and square the result $(x_i - \bar{x})^2$:

* $(88 - 85.91)^2 \approx 4.37$
* $(92 - 85.91)^2 \approx 37.09$
* $(79 - 85.91)^2 \approx 47.75$
* $(85 - 85.91)^2 \approx 0.83$
* $(95 - 85.91)^2 \approx 82.63$
* $(81 - 85.91)^2 \approx 24.11$
* $(86 - 85.91)^2 \approx 0.01$
* $(90 - 85.91)^2 \approx 16.73$
* $(83 - 85.91)^2 \approx 8.47$
* $(77 - 85.91)^2 \approx 79.39$
* $(89 - 85.91)^2 \approx 9.55$

Sum of squared differences $\approx 310.91$
Now, divide by $N-1$ (which is 10) and take the square root:


$$\sigma = \sqrt{\frac{310.91}{10}} = \sqrt{31.091}$$

$$\sigma \approx 5.58$$

**Original Results:**

* **Mean:** 85.91
* **Standard Deviation:** 5.58

---

### **3. Determination: Part 2 (Removing Outliers)**

Now we remove the highest and lowest scores.

* Lowest score: **77**
* Highest score: **95**

**New Data ($N = 9$):**
Scores: 88, 92, 79, 85, 81, 86, 90, 83, 89

**Step A: Calculate the New Mean**
Sum of the new scores: $88 + 92 + 79 + 85 + 81 + 86 + 90 + 83 + 89 = 773$


$$\bar{x}_{\text{new}} = \frac{773}{9}$$

$$\bar{x}_{\text{new}} \approx 85.89$$

**Step B: Calculate the New Standard Deviation**
Calculate the squared differences using the new mean (85.89) for the 9 remaining scores, sum them up, divide by $N-1$ (which is $9 - 1 = 8$), and take the square root.

* Sum of new squared differences $\approx 148.89$

$$\sigma_{\text{new}} = \sqrt{\frac{148.89}{8}} = \sqrt{18.611}$$


$$\sigma_{\text{new}} \approx 4.31$$



**New Results:**

* **Mean:** 85.89
* **Standard Deviation:** 4.31

### **Final Answer Summary**

* **Original Data:** Mean = **85.9**, Standard Deviation = **5.6**
* **Trimmed Data:** Mean = **85.9**, Standard Deviation = **4.3**

*(Notice how removing the extreme values barely changed the average/mean, but significantly lowered the standard deviation, proving that the dataset became more tightly clustered).*
