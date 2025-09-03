# Walmart Black Friday Spending Analysis                                                                                 



### **Project Overview**

This project analyzes customer purchase behavior at Walmart during the Black Friday sales event. The primary objective is to understand if spending habits differ across various demographic factors, such as **gender**, **marital status**, and **age**. By leveraging statistical methods like **Confidence Intervals** and **Central Limit Theorem**, this analysis provides data-driven recommendations to help Walmart's management make better business decisions.

***

### **Problem Statement**

The management team at Walmart Inc. wants to analyze customer purchase behavior, specifically the `Purchase` amount, against various demographic factors. The main questions to be answered are:

- Do spending habits differ between male and female customers?
- Are women spending more on Black Friday than men?
- How do purchasing patterns vary across different age groups and marital statuses?

***

### **Dataset**

The analysis is based on the `Walmart_data.csv` dataset, which contains transactional data from customers who purchased products during Black Friday. The dataset includes the following features:

| Column | Description |
| :--- | :--- |
| `User_ID` | Unique identifier for the customer |
| `Product_ID` | Unique identifier for the product |
| `Gender` | Sex of the user (F, M) |
| `Age` | Age in bins (e.g., 26-35, 51+) |
| `Occupation` | Occupation (masked) |
| `City_Category` | Category of the city (A, B, C) |
| `StayInCurrentCityYears` | Number of years staying in the current city |
| `Marital_Status` | Marital Status (0: Unmarried, 1: Married) |
| `ProductCategory` | Product Category (masked) |
| `Purchase` | Purchase Amount |

***

### **Methodology and Concepts**

The project follows a structured data analysis pipeline, including:

- **Exploratory Data Analysis (EDA):** Initial data inspection, including handling missing values, detecting outliers, and performing univariate and bivariate analysis to understand data distribution and relationships.
- **Statistical Inference:**
    - **Central Limit Theorem (CLT):** Used to compute confidence intervals, allowing us to infer population-level spending habits from a sample of data.
    - **Confidence Intervals:** Calculated for average purchase amounts across different groups (`Gender`, `Marital_Status`, `Age`) to determine if the population averages are statistically different.

***

### **Key Findings and Insights**

### **Observations:**

- **Gender:** The confidence intervals for average male and female purchase amounts **did not overlap**, indicating a statistically significant difference in spending.
- **Marital Status:** The confidence intervals for married and unmarried individuals **overlapped**, suggesting there is no statistically significant difference in their average spending across the entire dataset.
- **Age:** The analysis showed varying degrees of overlap between the confidence intervals of different age groups. Notably, the **0-17 age group** had no overlap with several other age groups, highlighting a distinct spending pattern. The **26-35 age group** represents the largest customer segment and has a significant impact on overall purchase amounts.

### **Recommendations:**

Based on the statistical analysis, here are actionable recommendations for Walmart's business strategy:

1.  **Leverage Gender Differences:** Since the analysis shows a significant difference in spending between genders, Walmart should:
    - **Analyze popular product categories** and brands among male and female customers.
    - **Develop targeted promotions and advertising** that appeal to each gender's interests.
    - **Consider optimizing store layouts** and product placements to cater to the shopping patterns of both genders.

2.  **Implement Age-Based Targeting:** The varying confidence interval overlaps among age groups highlight the need for a segmented approach. Walmart should:
    - **Develop marketing campaigns and product assortments** that resonate with the specific spending habits and preferences of different age segments.
    - **Focus on optimizing offerings** for age groups with higher average spending or those showing distinct purchasing behaviors, such as the 0-17 group.

3.  **Further Analysis on Marital Status:** While the overall analysis showed no significant difference, Walmart should not disregard this demographic. Further analysis within specific product categories or in combination with other factors like age and location might reveal valuable insights for more targeted strategies.

***

### 👨‍💻 **Technical Details**

- **Language:** Python
- **Libraries:** pandas, numpy, matplotlib, seaborn, scipy
- **Environment:** Google Colab
- **Repository Link:** `https://github.com/ramanujar12-com/walmart`

***

### **How to Run the Project**

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/ramanujar12-com/walmart.git](https://github.com/ramanujar12-com/walmart.git)
    ```
2.  **Navigate to the project directory:**
    ```bash
    cd walmart
    ```
3.  **Open the Google Colab file (`.ipynb`):**
    - You can open it directly in Google Colab.
4.  **Install the required libraries** (if not already installed):
    ```bash
    pip install pandas numpy matplotlib seaborn scipy
    ```
5.  **Run the notebook cells sequentially** to replicate the analysis and view the results.
