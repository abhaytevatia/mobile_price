# Mobile Price Range Prediction

## Problem Statement
In the competitive mobile phone market, companies want to understand sales data of mobile phones and factors that drive the prices. Mobile phones come in all sorts of prices, features, specifications, etc., and estimating the price of mobile phones is an important part of consumer strategy.

The objective of this project is to find out some relation between features of a mobile phone and its selling price. In this problem, we do not have to predict the actual prices but a price range indicating how high the price is. The dataset contains 2000 records of mobile phone information with 20 features, which is a mix of categorical features and numerical features.

## Data Description
The dataset contains 2000 records and 21 features, which consist of:

- Battery_power: Total energy a battery can store in one time measured in mAh.
- Blue: Has bluetooth or not.
- Clock_speed: Speed at which the microprocessor executes instructions.
- Dual_sim: Has dual sim support or not.
- Fc: Front camera megapixels.
- Four_g: Has 4G access or not.
- Int_memory: Internal memory in gigabytes.
- M_dep: Mobile depth in cm.
- Mobile_wt: Weight of the mobile phone.
- N_cores: Number of cores of the processor.
- Pc: Primary camera megapixels.
- Px_height: Pixel resolution height.
- Px_width: Pixel resolution width.
- Ram: Random Access Memory in megabytes.
- Sc_h: Screen height of mobile in cm.
- Sc_w: Screen width of mobile in cm.
- Talk_time: Longest time that a single battery charge will last when you are talking over the phone.
- Three_g: Has 3G access or not.
- Touch_screen: Has touch screen or not.
- Wifi: Has wifi or not.
- Price_range: This is the target variable with values of 0 (low cost), 1 (medium cost), 2 (high cost), and 3 (very high cost).

## Data Exploration
The distribution of the target variable shows us that the classes are almost balanced as the difference between the classes is minimal. Thus, we know that there's no class imbalance problem here. All the classes have around 450 records.

The distribution of the categorical features is almost similar to each other except the feature 'three_g,' which contains very few mobile phones that do not have 3G access. We can infer that almost all phones have 3G access if not 4G.

Most of the numerical features follow a uniform distribution except a few features like fc, px_height, and sc_w follow a right-skewed distribution.

The distribution of categorical features across different price ranges stays the same. There is a slight increase in the count of mobile phones in the very high-cost category for each categorical feature. Thus, we can infer that the more we pay, the more choices we can get.

The distribution of the numerical features across different price ranges shows us that only the features RAM, battery power, px_height, and px_width increase with an increase in price. These features are the most influential in determining the price ranges.

RAM has the strongest correlation with the target variable followed by battery power, px_height, and px_width. The rest of the numerical features have very low correlation with the target variable.

## Approach
- EDA and Feature Selection
- Removed Multicollinearity.
- Feature Selection.
- Splitting Dataset into train and test set.
- Model Training.
- Model Evaluation.

## Learning Outcome
The students will get a better understanding of how the variables are linked to each other and how the EDA approach will help them gain more insights and knowledge about the data that we have and classify the data into similar groups using Naive Bayes. They will also learn about how to choose important features using Random Forest.

![Image Alt Text](https://drive.google.com/file/d/1EJ2MO3frxZJIgZr_ttJ-5UrZhayw-8Ba/preview)

iStockPhoto - [Link](https://www.istockphoto.com/photo/cartoon-illustration-for-fun-concept-on-mobile-phone-themes-pixel-art-vintage-style-gm1132817705-612361670)

