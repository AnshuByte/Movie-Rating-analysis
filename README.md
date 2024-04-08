
# Movie Rating Analysis Project

## Overview
This project involves analyzing movie ratings data to derive insights into audience preferences and trends. Various analytical techniques are applied to explore factors influencing movie ratings and to identify patterns in audience behavior.

## Data Analysis Tasks

1. **Display Top 10 Rows of the Dataset**
   ```python
   data.head(10)
   ```

2. **Check Last 10 Rows of the Dataset**
   ```python
   data.tail(10)
   ```

3. **Find Shape of the Dataset (Number of Rows and Number of Columns)**
   ```python
   data.shape
   print('Number of Rows:', data.shape[0])
   print('Number of Columns:', data.shape[1])
   ```

4. **Getting Information About Our Dataset Like Total Number Rows, Total Number of Columns, Datatypes of Each Column And Memory Requirement**
   ```python
   data.info()
   ```

5. **Check Null Values in the Dataset**
   ```python
   data.isnull().sum()
   sns.heatmap(data.isnull())
   plt.show()
   ```

6. **Drop All the Missing Values**
   ```python
   data = data.dropna(axis=0)
   sns.heatmap(data.isnull())
   plt.show()
   ```

7. **Check for Duplicate Data**
   ```python
   dup_data = data.duplicated().any()
   print("Are there any duplicated values in data?", dup_data)
   ```

8. **Get Overall Statistics About the DataFrame**
   ```python
   data.describe()
   ```

9. **Display Title of The Movie Having Runtime >= 180 Minutes**
   ```python
   data[data['Runtime (Minutes)'] >= 180]['Title']
   ```

10. **In Which Year There Was the Highest Voting?**
    ```python
    sns.barplot(x='Year', y='Votes', data=data)
    plt.title("Votes By Year")
    plt.show()
    ```

like this we have done more comparisions... 

## Conclusion
This README provides an overview of the data analysis tasks performed on the IMDB movie dataset. Each task is accompanied by the corresponding Python code snippet. By analyzing various aspects such as movie ratings, runtime, and revenue, valuable insights have been gained into audience preferences and trends in the movie industry.

## Future Work
- Explore additional data analysis tasks to uncover more insights from the dataset.
- Conduct further research on specific trends identified in the analysis.
- Utilize machine learning techniques to predict movie ratings or revenue based on various attributes.

