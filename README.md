# AirBnB Listings in Munich: An Analysis  

This analysis is based on a dataset containing AirBnB listings and their respective prices.
Based on available listing information, the effect of seasonality, location and other factors is explored.
While price seasonality and appartment location are mostly explored using visualizations, other factors such as amenities and host ratings are used as input for a machine learning model.

# Data

All data is taken from the Inside Airbnb website:
http://insideairbnb.com/get-the-data/

To start the analysis yourself, download the Munich dataset from the website and adjust the csv import accordingly.  

	df_listings = pd.read_csv(f"C:/example_path/muc_listings.csv")  
	df_cal = pd.read_csv(f"C:/example_path/muc_calendar.csv")



# Libraries

The following libraries are required to run the code:

		import numpy as np
		import pandas as pd
		import matplotlib.pyplot as plt
		from IPython.display import display, HTML
		import plotly.express as px
		from datetime import datetime as dt
		# from pandas_profiling import ProfileReport
		import seaborn as sns

		from sklearn.preprocessing import MultiLabelBinarizer
		from sklearn.linear_model import LinearRegression
		from sklearn.model_selection import train_test_split
		from sklearn.metrics import r2_score, mean_squared_error



# Description of files in repository

File Name	  										| File Description
-------------										| -------------
munich_airbnb_analysis.ipynb  						| Jupyter Notebook containing the whole analysis.
README.md											| Readme file.
plots/Apartment_Price_Heatmap.png					| Heatmap of apartment prices in Munich.
plots/Neighbourhoods_Prices.png						| Plot of average apartment prices per neighborhood.
plots/Neighbourhoods_Prices.html					| Interactive HTML version of the plot.
plots/Unique_Amenities.png							| Distribution of unique amenities for apartment listings in Munich.
plots/Wordcloud_Oktoberfest.png						| Wordcloud generated from listing titles.
plots/Plot_Price_per_Night_by_Scraping_Date.png		| Plot of prive averages separated by data scraping date.

