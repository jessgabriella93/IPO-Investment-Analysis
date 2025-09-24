## IPO Investment Analysis  

This project applies **machine learning** to predict whether an IPO (Initial Public Offering) is a **good or bad investment**. Using the S&P 500 as the benchmark, IPO details, CEO attributes, and sector/industry indicators, the model evaluates post-IPO performance to guide investment decisions.  

## Process  

**Data Preparation**  
  - Cleaned missing values, standardized categorical labels, and formatted dates/financial fields.  
  - Engineered features such as **5-day, 30-day, and 90-day returns** after IPO.  

**Target Definition**  
  - 2 = Good investment - Outperformed the S&P 500 for ≥90 days or had positive 90-day return.  
  - 1 = Bad investment  

**Modeling**  
  - Trained a **Random Forest Classifier** with an 80/20 train-test split.  
  - Evaluated results using classification report and confusion matrix.  

## Results  

**Accuracy:** 93% overall  
**Good investments (Class 2):** Precision 94%, Recall 97%, F1-score 0.96  
**Bad investments (Class 1):** Precision 78%, Recall 61%, F1-score 0.69
**Top features:** trading volume Day 1, close price Day 0, trading volume Day 0, Year, and the number of days stocks are profitable  

## Insights  

- **Public Utilities** stood out as the sector most likely to yield strong IPOs.  
- The model is highly effective at identifying profitable IPOs but less reliable for predicting weak ones.  
- Future improvements could include class balancing and experimenting with alternative algorithms.  

## Tech Stack  

- **Python** (pandas, numpy, scikit-learn, matplotlib, seaborn)  
- **Machine Learning** (Random Forest Classifier)  
- **Visualization** (feature importance, sector analysis) 
