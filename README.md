# All-Weather-Portfolio-Reconstucted

#### This project presents a modification of Ray Dalio's "All Weather Portfolio" using Machine Learning techniques, specifically Natural Language Processing (NLP) and Topic Modeling. We maintain the same portfolio asset class composition as Bridgewater Associates has proposed on its website, but we adapt the weights of the assets in the portfolio in response to economic regime shifts, as identified by our Machine Learning model.

#### The original "All Weather" portfolio, which targets investors with a long-term investment horizon, consists of four distinct baskets, each comprising a different combination of asset classes. This design serves as a diversification mechanism. The original portfolio suggests the rebalancing of portfolio weights according to "rising" or "falling" market expectations and "growth" or "inflationary" economic regime.

#### In our approach, we employ Word2Vec word embedding techniques to identify the key terms "Inflation" and "Growth" in Federal Reserve speech transcripts and VIX as market volatility guage to determine market expectation. The word terms are used as features to train our model. We conducted Sentiment Analysis on Federal Reserve speech transcripts dating from 1996 to 2022 using Machine Learning techniques, Natural Language Processing (NLP), and Latent Dirichlet Allocation (LDA) Topic Modeling to inform our portfolio rebalancing strategy for different economic regimes.

![All Weather Portfolio Composition](https://github.com/swhy0913/All-Weather-Portfolio-Reconstucted/assets/19575677/ac1f63b9-5526-4981-ae9e-b5a5c9761162)

## The following are the model performance comparison:

| Fed Speech Transcript using Word2Vec (2006 - 2022): |                  |
|-----------------------------------------------------|------------------|
| Sharpe Ratio                                        | 0.95             |
| CAGR(%)                                             | 5.21             |
| Max DD(%)                                           | 279 days, -20.28 |
| Std Deviation(%)                                    | 5.0              |

#### Benchmark comparison: 

| "All Weather Portfolio" by Bridgewaters Assoc. (2003 - 2023): |                  |
|---------------------------------------------------------------|------------------|
| Sharpe Ratio                                                  | 0.73             |
| CAGR(%)                                                       | 6.71             |
| Max DD(%)                                                     | 9 months, -20.19 |
| Std Deviation(%)                                              | 7.6              |

(Source: https://www.lazyportfolioetf.com/allocation/)

#### Benchmark comparison: 

| S&P500 (2003 - 2023): |                   |
|-----------------------|-------------------|
| Sharpe Ratio          | 0.60              |
| CAGR(%)               | 9.93              |
| Max DD(%)             | 16 months, -50.80 |
| Std Deviation(%)      | 14.67             |

(Source: https://www.lazyportfolioetf.com/allocation/)
