# Using deep learning models to predict the price movement of the Bulgarian Stock Exchanges SOFIX Index

## I utilise deep learning models to build a long/short strategy that outperforms simply "going long" the SOFIX Index

## 🚨 Important Disclaimer 🚨 

*This project was embarked upon as a personal exploration and for enjoyment, with the primary goals of deepening my understanding of neural networks and advancing my machine learning capabilities through practical application. It represents an exercise in applying theoretical knowledge rather than a definitive guide or strategy for outperforming any financial index, such as the SOFIX index.*

*The insights and outcomes presented are part of my learning journey and should not be interpreted as professional investment advice or as a reliable method for generating market alpha. While every effort has been made to ensure the accuracy and completeness of the project, it's important to acknowledge the potential for oversight or error. This endeavor is shared in the spirit of learning and should be viewed as such by its audience.*


## Deep Learning Long/Short Strategy Performance:

![Deep Learning Long/Short Strategy Performance](https://raw.githubusercontent.com/evgeni-g-georgiev/Bulgarian_Stock_Market_Price_Prediction/master/DeepLearningStrategyPerformance.png)

## Brief Project Overview

As mentioned earlier, this project utilizes deep learning models to predict the price movement of the Bulgarian Stock Exchanges SOFIX Index and to build a long/short strategy that will aim to outperform going simply long the SOFIX Index.

## Data Collection and Preparation

The project includes three main datasets:

**Intraday Data:** Captures minute-by-minute price data from the SOFIX Index between Jan 3, 2023, and Feb 2, 2024.
**Up/Down Data:** Indicates whether the index opens higher or lower compared to the previous day's closing level, from Jan 4, 2023, to Feb 5, 2024.
**Closing Levels:** Contains the closing levels of the SOFIX Index for each date.
The mapping of intraday data to up/down data is crucial for training the model to predict the index's opening direction for the next day, considering market behaviors from the previous day.

### Model Building and Selection

The deep learning model is built from scratch, incorporating LeakyReLU activation functions and a segmented layer configuration to enhance performance. Multiple architectures are tested, with key parameters such as layer configuration and learning rates optimized.

Models are evaluated based on accuracy and loss metrics, with a focus on cross-validation performance. The top-performing models are selected for further analysis, considering both accuracy and loss values.

### Evaluation and Strategy Development

The performance of selected models is evaluated using a simple investment strategy. The strategy involves buying or selling the index based on the model's predictions of whether the index will open higher or lower.

The effectiveness of the strategy is compared to traditional long-only investment approaches. Despite potential fluctuations in accuracy, the strategy aims to capitalize on significant price movements, potentially outperforming conventional investment methods.

## How do I run the code myself?

Unfortunately, the code will not be fully executable for most users.

This is because some of the data used is only available through purchase directly from the Bulgarian Stock Exchange, as per my usage agreement with the BSE, I am not permitted to distribute the data in its original format.

You can contact the BSE directly if you wish to purchase the data and run the code yourself: https://www.bse-sofia.bg/en/contact-us

Regardless, I have made an effort to make the code and my methodology as interpretable as possible and to visualize all relevant results so that you don't really need to be able to run the code to follow along!

A quick rundown of the different files and folders:

- **"sofix_price_prediction.ipynb":** This is the main Jupyter Lab file where I include my code, methodology, and all relevant results and visualisations.
- **"final_model_candidates":** This folder contains the 100 neural network models I build and discuss in my code. 
- **DeepLearningStrategyPerformance.png:** A graph depicting the performance of the best deep learning model long/short strategy.


## Some Final Comments...

So, what I have built is a methodology that produces several deep learning models all of which produce outputs that can be leveraged to build an investment strategy that can outperform going simply long the SOFIX Index.

I think that is pretty cool 😊
