**Step 1:** Before I begin assessing our data for missing values, it is important that I understand the ethical implications surrounding data processing. To best prepare myself for this module, I reviewed one or more of the following resources:

Data Science Ethics Flashcard Video Series
What Do I Need to Understand about Data Ethics?
Introduction to Data Cleaning

**Step 2:** Check the dataset for missing values.

```
#TODO: Leverage the isnull() and sum() functions to find the number of missing values in each column
missing_values = data.isnull().sum()

#TODO: Turn the missing value counts into percentages
missing_values_percentage = (missing_values/ len(data)) * 100

#TODO: Return counts and percentages of missing values in each column
missing_data = pd.DataFrame({'Missing Values': missing_values, 'Percentage (%)': missing_values_percentage})
missing_data.sort_values(by='Percentage (%)', ascending=False)
```

<img width="531" alt="Screenshot 2025-01-29 at 4 39 53 PM" src="https://github.com/user-attachments/assets/42524277-d4a1-4a14-926d-7debad871c2a" />
