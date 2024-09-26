# DataAnalytics_Project-_Global_Superstore
### In the first step, you imported the necessary libraries for data manipulation and analysis:
import pandas as pd
import numpy as np
pd.set_option('display.min_rows', 50)  # Adjusts display settings to show more rows

df.info()
df.describe()
### converted the Order Date and Ship Date columns from string format to datetime objects and configured the display settings for better readability.

df['Order Date'] = pd.to_datetime(df['Order Date'], errors='coerce')  # Convert to datetime, coercing errors

df['Ship Date'] = pd.to_datetime(df['Ship Date'], errors='coerce')  # Convert to datetime, coercing errors

df[['Order Date', 'Ship Date']]  # Display the converted columns


