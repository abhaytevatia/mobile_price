# Mobile Price Range Prediction

## Problem Statement
In the competitive mobile phone market, companies aim to comprehend mobile phone sales data and the key factors influencing prices. Mobile phones come in various price ranges, each offering distinct features and specifications, making price estimation a critical aspect of consumer strategy.

The objective of this project is not to predict exact prices, but to determine the price range, indicating the price's relative level. The dataset comprises 2000 records of mobile phone details, encompassing 20 features that combine both categorical and numerical attributes.

## Data Description
The dataset consists of 2000 records and 21 features, including:

- Battery_power: Battery capacity measured in mAh.
- Blue: Bluetooth availability.
- Clock_speed: Microprocessor execution speed.
- Dual_sim: Dual SIM card support.
- Fc: Front camera resolution (megapixels).
- Four_g: 4G network support.
- Int_memory: Internal memory (gigabytes).
- M_dep: Mobile depth (cm).
- Mobile_wt: Mobile phone weight.
- N_cores: Number of processor cores.
- Pc: Primary camera resolution (megapixels).
- Px_height: Pixel resolution height.
- Px_width: Pixel resolution width.
- Ram: Random Access Memory (megabytes).
- Sc_h: Screen height (cm).
- Sc_w: Screen width (cm).
- Talk_time: Maximum talk time on a single battery charge.
- Three_g: 3G network support.
- Touch_screen: Touchscreen availability.
- Wifi: WiFi support.
- Price_range: Target variable, representing price categories (0: low cost, 1: medium cost, 2: high cost, 3: very high cost).

## Data Exploration
The distribution of the target variable reveals balanced classes, minimizing class imbalance concerns. Each class contains approximately 450 records.

Categorical feature distributions are consistent, except for 'three_g,' with very few phones lacking 3G access. We can infer that most phones support 3G, if not 4G.

Numerical feature distributions are uniform, except for a few right-skewed features like fc, px_height, and sc_w.

Categorical feature distributions across price ranges remain consistent, with a slight increase in very high-cost phones for each category. Higher prices offer more choices.

Numerical features associated with price ranges show that RAM, battery power, px_height, and px_width increase with price. These features strongly influence price ranges.

RAM demonstrates the strongest correlation with the target variable, followed by battery power, px_height, and px_width.

## Approach
- Exploratory Data Analysis (EDA) and Feature Selection.
- Multicollinearity Removal.
- Feature Selection.
- Dataset Splitting into Train and Test Sets.
- Model Training.
- Model Evaluation.

## Learning Outcome
This project will enhance understanding of variable relationships and the role of EDA in deriving insights and classifying data using Naive Bayes. It also covers feature selection using Random Forest.
