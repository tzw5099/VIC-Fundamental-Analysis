## VIC NLP Analysis and Modeling
#### Problem
Can professional investors consistently outperform the market? Yes!* (*not accounting for risk)
How can we employ fundamental valuation investment write-ups in order to reliably identify investments that will outperform the market?

#### Data
- **[ValueInvestorsClub.com Beautiful Soup Scrape](./code/Website scrape.ipynb)**
- Performance relative to market (over one year)
- Write-up sentiment
- TF-IDF, key-word findings
- Valuation metrics (P/E, P/Sales, ROC, etc)

#### Hypothesis
A combination of “cheap” valuation metrics and certain TFIDF weights should correlate with higher than market returns over a one year time period, on average. Given the high ratio of signal to noise in this application, even a low ROC AUC score greater than .5 should contribute to achieving better-than-market returns.

#### Conclusion
A classifier model with an AUC of between 0.58-0.60 is capable of reliably identifying better than average write-ups from the entire sample space, on average. While all long write-ups from VIC have an average return premium of 0.8%, our models have an average return premium of greater than 9%, on average.

#### Future steps
- Topic modeling (LDA)
- Aspect based sentiment analysis
- Further crowdsourcing of fundamental valuation investment write-ups
- Extra model tuning
- Time Series exploration
- ROI optimization (in contrast with current buy-and-hold for 1 year method)
- Scrape message content as added feature
- Automated trading algorithm deployed into simulated trading environment
