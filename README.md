# Car Analytics using Regression
![Northside-Honda_MG_9908-](https://user-images.githubusercontent.com/110783008/202796331-bcf70117-f3a7-428a-899a-58a7a00cbf6f.jpeg)
## Scope:
- Help car Dealers and Retailers to recommend car prices based on the features the customer wants</br>
- Create a model that predicts the car prices .


## Data:
The data has been web scraped from  https://www.cars.com/
Rows = 8840 , Columns = 10  

## Files:
The repository has the following files:<br/>
- Data folder : This folder consists of the csv files, that are being used in the different files throughout the project<br/> 
- Data Scraping & Data Cleaning :  This notebook, consists of the web scraping process and data cleaning</br>
- EDA : This notebook involves Exploratory Data Analysis on the cleaned data </br>
- Modelling 1 : This notebook, consists of the code evaluating the Base model, which is Ridge Regression</br>
- Modelling 2 : This notebook, consists of the code that deals with evaluating the model performances on the train and test sets</br>

## Project Details:
Data Scraping: The data for this project has been web scrapped from https://www.cars.com/.</br>
- The Data has been webscraped using BeautifulSoup</br>
- After getting all the data into a list, it was then converted into a datframe using pandas.</br>
Features: Mileage,	Rating,	Rating-Count,	Year,	Price	Name,	Status,	model_details,	Class,	Version1, Version2</br>
Data Modelling:</br>
- All the data was processed by OneHotEncoding and then standardised through sklearn pipeline </br>
- GridsearchCV was further cross validation</br>
- The regression models used in this project are:</br>
  - Ridge 
  - Lasso 
  - KNeighborsRegressor
  - RandomForestRegressor
  - XGBRegressor
- The best performing model was Lsso, with a accuracy score of 94%</br>
- Model metrics:</br>
<img width="316" alt="Screen Shot 2022-11-17 at 12 28 38 PM" src="https://user-images.githubusercontent.com/110783008/202801897-b1c55bde-56ef-4444-ab27-db3698dadcbb.png"></br>
- Regplot that shows the prediction on the train and test set:</br>
<img width="984" alt="Screen Shot 2022-11-17 at 12 33 34 PM" src="https://user-images.githubusercontent.com/110783008/202802049-d49ec14f-f5f6-4d23-859e-4f40bdf519f0.png"></br>

## Summary:
- The Best model has a 94% accuracy.
- The model predicts well.
- This model can be used by car dealers to predict prices and recommend theirs customers with the cars they should buy.

