# exp-15

# **Experiment 15: Data Normalization and Data Type Conversion**

---

## **Aim**
To use Python to scale numerical data and convert categorical text into numbers so that a machine learning model can process the dataset accurately.

---

## **Theory**

Data preprocessing is the process of cleaning and organizing raw data. Since different features often use different units or formats, we use two main techniques to fix them:

### **1. Data Normalization**
This is used to put all numbers on the same scale. For example, if one column has values from 1 to 10 and another has values from 1,000 to 10,000, the model might think the larger numbers are more important. Normalization fixes this.

- **Min-Max Normalization:** This squashes all values into a small range, usually between 0 and 1.  
- **Z-Score Normalization:** This centers the data around zero based on the average value. It is helpful when your data has extreme high or low values (outliers).  
- **Decimal Scaling:** This simply moves the decimal point to make the numbers smaller and easier to manage.  

---

### **2. Data Type Conversion (Encoding)**
Computers are good at math but bad at understanding words like "Mumbai" or "Electronics." Encoding turns these words into numbers.

- **Label Encoding:** This gives every category a number (e.g., 0, 1, 2). It's simple but can accidentally make the computer think "2" is better than "0."  
- **One-Hot Encoding:** This creates new columns for each category and uses 1s and 0s to show which one is active. This is the "gold standard" for categories that don't have a specific rank.  
- **Dummy Encoding:** This is a shortcut version of One-Hot encoding that removes one extra column to keep the data efficient.  

---

## **Conclusion**

By writing these codes, I learned how to prepare a raw dataset for analysis.  

1. **Scaling Results:** I found that **Min-Max scaling** worked best for keeping my data within a clean 0-to-1 range, while **Z-Score** was better for seeing how far a value was from the average.  

2. **Encoding Results:** I realized that **Label Encoding** is fine for simple "Yes/No" data, but **One-Hot Encoding** is necessary for columns like "Department" or "City" so the computer doesn't get confused by the order of the numbers.  

3. **Efficiency:** Using professional libraries like `Scikit-learn` and `Pandas` makes it much faster to process large files, like the Amazon and Student datasets, compared to doing the math manually.  

---

Do you have any more experiments left in this series, or is this the final one for your Python lab?
