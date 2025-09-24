The purpose of my Capstone project was to predict property prices in specific areas of Liverpool. 

Why Liverpool?  - After attending the Property Investor show at the Excel centre in London, I attended a one-day workshop with Dominic Farrell regarding below market value property investing In Liverpool Distressed Assets | Property Investments | Property Sourcing | Off-Market Deals

As part of my retirement planning, I would like to attend property auctions in Liverpool in the very near future with a view to buying below market value properties for investment purposes. This Machine Learning project and the knowledge that I gained from Domnics course should assist me in this respect.

I sourced a Dataset on Kaggle:UK_Property_Sale_Prices_and_EPC_Energy_Efficiency

It is a large dataset ~ 2GB and it was therefore not possible to upload it to my GitHub repository:khanms67/Imperial-College-Capstone-Project

My Python code file is: MSK_Property_Price_Prediction_Portfolio_Project.ipynb

In my code, I explored the shape of the dataset. There were 5769140 rows and 98 columns.

I decided to keep just 18 columns of data for my project. These columns were based upon Location, Energy Metrics and Structural features.

After further analysis, I dropped 4326855 rows from the dataset that were missing a property price.

I then extracted specific Liverpool postcodes from the remaining data. An example of such data can be found in the Liverpool_properties spreadsheet which has also been uploaded to GitHub.

I selected input features such as Postcode prefix, Property type (House, Flat, Bungalow etc), Type of property (Detached, Semi-detached, terrace etc) and the sale date to train selected machine learning models to predict house prices for the specific Liverpool post codes.

The Machine Learning models that I selected were Linear Regression, RandomForestRegressor, GradientBoostingRegressor and XGBoost. I then used GridSearchCV to tune the hyperparameters that affect how the model learns.

I did experiment by adding another input parameter (Number of Habitable rooms) to see what effect that had on my models performance. 

I found that XGBoost performed the best before and after hyper parameter tuning.

After introducing an additional input parameter, the performance of XGBoost improved further in the hyper parameter tuning phase.

The detailed metrics can be found by running the python code – each step is fully documented within the file (MSK_Property_Price_Prediction_Portfolio_Project.ipynb).

The project was constructed in a week and had time permitted, I would have experimented further to see if I could improve the models performance even more. The results strongly suggest that further improvements can be made.

I look forward to enhancing this first iteration of a property price predictor.
