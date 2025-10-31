Flight Fare Analytics using Python

This project focuses on analyzing flight ticket prices to uncover insights into how various factors — such as airline, source city, travel class, and booking time — influence airfare.  
Using Python’s data analysis and visualization tools, the project explores price patterns, builds visualizations, and derives meaningful insights that can help both customers and businesses understand flight pricing behavior.

Dataset

Source: [Kaggle – Flight Price Prediction Dataset](https://www.kaggle.com/datasets/shubhambathwal/flight-price-prediction)

Columns:
| Column | Description |
|--------|--------------|
| `airline` | Name of the airline |
| `flight` | Flight number/code |
| `source_city` | City of origin |
| `departure_time` | Departure time category (Morning, Evening, etc.) |
| `stops` | Number of stops |
| `arrival_time` | Arrival time category |
| `destination_city` | Destination city |
| `class` | Type of ticket (Economy / Business) |
| `duration` | Total duration of the flight (in hours) |
| `days_left` | Number of days left before departure |
| `price` | Ticket price (target variable) |

Project Objectives

- Analyze how **airline**, **class**, and **booking timing** affect flight prices.  
- Identify **which airlines are most/least expensive**.  
- Study the **impact of advance booking** on flight fare.  
- Compare **Economy vs Business** ticket pricing patterns.  
- Visualize flight pricing trends using data-driven insights.

Tools & Libraries Used

- **Python 3.10+**  
- **Pandas** – Data manipulation and analysis  
- **NumPy** – Numerical computations  
- **Matplotlib** & **Seaborn** – Visualization  
- **Jupyter Notebook** – Interactive environment  

Exploratory Data Analysis (EDA)
1. Average Flight Price per Airline
```python
sns.barplot(x='airline', y='price', data=df, estimator='mean', errorbar=None)
