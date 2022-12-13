# ESG Investment Portolio Under New COVID-19 Prevention Stage in China

## General information
- **Author**: Haoyang Yu, Applied Mathematics & Computational Sciences, Class of 2024, Duke Kunshan University
- **Instructor**: Prof. Luyao Zhang, Duke Kunshan University
- **Disclaimer**: Submissions to the Final Project for [STATS201 Introduction to Machine Learning for Social Science, 2022 Autumn Term (Seven Week - Second)](https://ms.pubpub.org/) instructed by Prof. Luyao Zhang at Duke Kunshan University.
- **Acknowledgments**: I would like to express my greatest gratitude to Prof. Luayo Zhang for her generous and inspiring instructions on STATS201: Instruction to Machine Learning for Social Science.
## Project Summary
- **Background & Motivation**:
As the symptom of Covid-19 Omicron is mild, the Chinese government has decided to ease the prevention policy, which includes canceling the travel code and nuclear test check in the public area. People’s travel will not be limited, in this case, the financial market may perform tendencies that are different from the pandemic. For the outperformance of the ESG portfolio, a refuge for investors during the pandemic, this project aims to figure out its advantages during the pandemic and predict its return under the new policy of Covid-19 prevention in China. The project will contribute to the application of machine-learning methods in market surveys and investment portfolio return prediction. The study considers capital flowing (spillover effects) into account, and thus it can provide a direction for the pricing and trading algorithms in a real-world implementation.
- **Research Questions**:
1.	Why the ESG portfolio outperforms during pandemic periods?
2.	What is the predictive performance of the ESG portfolio under the new Covid-19 prevention stage in China?
- **Application Scenario**: 
Our raw input variables: The historical time-series data of capital flow from Defense and EAFE portfolios to ESG portfolio, and the historical data of the returns of the three portfolios.
- **Portfolios Data**: Our data set are from [MSCI](https://www.msci.com/). We include close price daily return from 1st May 2017 to 1st May 2020 in the dataset.
- **Methodology**: 
The MSCI reports portfolio return spreads (long minus short portfolio returns) in the form of an index for the respective safer investment strategies. In the present study, the continuously compounding gross index returns are computed for the respective indices, i.e. Rt = Ln (Pt / Pt-1) *100. Here, Rt is the daily return, Ln is the logarithmic term, Pt is the current day's index price and Pt-1 is the previous day's index price. The respective indices are re-balanced periodically, such as a monthly basis for the EAFE and defensive portfolios, and quarterly for the ESG portfolio. These index returns have been further used in generating the net pairwise spillover effects.
In the prediction part, use ARIMA model to learn the relationship between historical ESG portfolio return and capital flow to ESG portfolio, then predict the return rate from 2021 to 2022.

- **Expected Results**: 
We are expecting a result of high capital flow to ESG portfolio comes with high return of ESG portfolio.

- **Intellectual Merit & Practical Impacts**: 
For the outperformance of the ESG portfolio, a refuge for investors during the pandemic, this project aims to figure out its advantages during the pandemic and predict its return under the new policy of Covid-19 prevention in China. The project will contribute to the application of machine-learning methods in market surveys and investment portfolio return prediction. The study considers capital flowing (spillover effects) into account, and thus it can provide a direction for the pricing and trading algorithms in a real-world implementation.

## Table of Contents
- [Data](https://github.com/Rising-Stars-by-Sunshine/Final_STATS201_Haoyang#data)
- [Code](https://github.com/Rising-Stars-by-Sunshine/Final_STATS201_Haoyang#code)
- [Spotlight](https://github.com/Rising-Stars-by-Sunshine/Final_STATS201_Haoyang#spotlight)
- [More about the Author](https://github.com/Rising-Stars-by-Sunshine/Final_STATS201_Haoyang#more-about-the-author)
- [References](https://github.com/Rising-Stars-by-Sunshine/Final_STATS201_Haoyang#references)

## Data
|                    |                                                    **Portfolio Data**                                                   |                       **Capital Flow Data**                      |
|--------------------|:----------------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------:|
| **Data Source**    |                       [MSCI](https://www.msci.com/)                       | [Amanjot Singh](https://www.sciencedirect.com/science/article/pii/S1544612320307583#sec0006) |
| **Queried Data**   |   [Return_Queried](https://github.com/Rising-Stars-by-Sunshine/Final_STATS201_Haoyang/tree/main/data)   |                                 -                                |
| **Processed Data** | [Return_Processed](https://github.com/Rising-Stars-by-Sunshine/Final_STATS201_Haoyang/tree/main/data) |                                 -                                |

## Code
- [Analytor](https://github.com/Rising-Stars-by-Sunshine/Final_STATS201_Haoyang/blob/main/code/Predictor.ipynb)

## Spotlight
- **Posters**:

![poster](https://github.com/Rising-Stars-by-Sunshine/Final_STATS201_Haoyang/blob/main/spotlight/Poster.png)
***Figure No.1**. Project Poster (created by [Canva](https://www.canva.com/design/DAFT-dVPBOM/fzR4WbsJPm6xCImV6BYMOA/view?utm_content=DAFT-dVPBOM&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton))*

## Contribution to the Literature:

<img src="https://github.com/Rising-Stars-by-Sunshine/Final_STATS201_Haoyang/blob/main/spotlight/Contribution%20to%20the%20Literature.png" height="500" alt="Contribution to Literature"/><br/>
***Figure No.2**. Contribution to the Literature (created by [Whimsical](https://whimsical.com))*

## Result:

<img src="https://github.com/Rising-Stars-by-Sunshine/Final_STATS201_Haoyang/blob/main/spotlight/Spillover17-20.png" height="300" alt="Spillover of portfolios from 2021-2022"/><br/>
***Figure No.3**. Spillover of portfolios from 2021-2022. For the defensive strategy, it is 53.6–52.5 = 1.1 percent, for the ESG strategy, it is 59.7–54.1 = 5.6 percent, and for the EAFE strategy, it is 44.3–37.7 = 6.6 percent. In general, the capital flows away from the defensive and ESG portfolios to the EAFE portfolio.*

<img src="https://github.com/Rising-Stars-by-Sunshine/Final_STATS201_Haoyang/blob/main/spotlight/distance%20fig.jpeg" height="300" alt="Return Rate distance fig"/><br/>
***Figure No.4**. This figure represents the distance of monthly return rate of EAFE and ESG China portfolio. i.e. The points above x-axis mean that the monthly return rate of EAFE is greater than ESG China, vice versa. The blue line is the predicted distance based on capital flow between ESG China and EAFE. (created by [ARIMA](https://www.machinelearningplus.com/time-series/arima-model-time-series-forecasting-python/))*

<img src="https://github.com/Rising-Stars-by-Sunshine/Final_STATS201_Haoyang/blob/main/spotlight/distance%20data.png" height="300" alt="Return Rate distance data"/><br/>
***Figure No.5**. In detail, we can see the monthly predicted values are almost positive, that just means the return rate of EAFE is greater than ESG China, which matches the results in figure 3: the capital flows away to EAFE in genenral.*

## More about the author:

Haoyang Yu’s research interests are the development of the trading algorithms, the financial derivatives research and industrial financial research. He is currently the interim executive co-chair of SciEcon AMA. He has also co-authored cryptocurrency’s market circulation-related research articles that are being prepared to submit to world-leading conferences. Besides his experience in SciEcon, he is a junior student at Duke Kunshan University majoring in Applied Mathematics & Computational Sciences. He also has rich working experience in financial industries, such as strategic consulting, management consulting and investment banking, etc. His last position was as a summer intern at PricewaterhouseCoopers during his sophomore-year summer break and he is currently an intern at a top Chinese brokerage (securities) company.

## Reference:

Broadstock DC, Chan K, Cheng LTW, Wang X. The role of ESG performance during times of financial crisis: Evidence from COVID-19 in China. Financ Res Lett. 2021 Jan;38:101716.

Bertrand and Lapointe, 2015 P. Bertrand, V. Lapointe How performance of risk-based strategies is modified by socially responsible investment universe? Int. Rev. Financ. Anal., 38 (2015), pp. 175-190 

Coudert and Gex, 2008 V. Coudert, M. Gex Does risk aversion drive financial crises? Testing the predictive power of empirical indicators J. Empir. Finance, 15 (2) (2008), pp. 167-184 

Diebold and Yilmaz, 2012 F.X. Diebold, K. Yilmaz Better to give than to receive: predictive directional measurement of volatility spillovers Int. J. Forecast., 28 (1) (2012), pp. 57-66 

Hamilton, 1989 J.D. Hamilton A new approach to the economic analysis of nonstationary time series and the business cycle Econometrica: J. Econom. Soc. (1989), pp. 357-384 

Hirshleifer, 2008 D. Hirshleifer Psychological bias as a driver of financial regulation Eur. Financ. Manage., 14 (5) (2008), pp. 856-874 

Kenourgios and Samitas, 2011 D. Kenourgios, A. Samitas Equity market integration in emerging Balkan markets Res. Int. Bus. Finance, 25 (3) (2011), pp. 296-307 

Schaller and Norden, 1997 H. Schaller, S.V. Norden Regime switching in stock market returns Appl. Financ. Econ., 7 (2) (1997), pp. 177-191 

Singh and Singh, 2016 A. Singh, M. Singh US financial conditions index and its empirical impact on information transmissions across US-BRIC equity markets The Journal of Finance Data Sci., 2 (2) (2016), pp. 89-111 

Koepke, 2018 R. Koepke Fed policy expectations and portfolio flows to emerging markets J. Int. Financ. Markets Inst. Money, 55 (2018), pp. 170-194 

Koutmos, 2018 D. Koutmos Return and volatility spillovers among cryptocurrencies Econ. Lett., 173 (2018), pp. 122-127 

Lehkonen and Heimonen, 2014 H. Lehkonen, K. Heimonen Timescale-dependent stock market comovement: bRICs vs. developed markets J. Empir. Finance, 28 (2014), pp. 90-103 

Lesser et al., 2016 K. Lesser, F. Rößle, C. Walkshäusl Socially responsible, green, and faith-based investment strategies: screening activity matters! Finance Res. Lett., 16 (2016), pp. 171-178 

Lins et al., 2017 K.V. Lins, H. Servaes, A. Tamayo Social capital, trust, and firm performance: the value of corporate social responsibility during the financial crisis J. Finance, 72 (4) (2017), pp. 1785-1824 

Nofsinger and Varma, 2014 J. Nofsinger, A. Varma Socially responsible funds and market crises J. Bank Financ., 48 (2014), pp. 180-193 

Singh, Amanjot. "COVID-19 and safer investment bets." Finance research letters 36 (2020): 101729.

Singh and Kaur, 2017 A. Singh, P. Kaur A short note on information transmissions across US-BRIC equity markets: evidence from volatility spillover index J. Quant. Econ., 15 (1) (2017), pp. 197-208 

Instructions for GitHub Readme:
https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax

Sample Code for Prediction:
https://github.com/Rising-Stars-by-Sunshine/stats201-tutorial-prediction

Yahoo Finance. (2022). The Kraft Heinz Company (KHC) Historical Data. Queried from https://finance.yahoo.com/quote/KHC/history?p=KHC

Zhang, L. (Sunshine). (2022). Machine Learning for Predictions. Machine Learning for Social
Science. Retrieved from https://ms.pubpub.org/pub/ml-prediction

Zhang, L. (Sunshine). (2022). Venues for Computer Security and Beyond. Machine Learning for
Social Science. Retrieved from https://ms.pubpub.org/pub/security

Zhang, L. (Sunshine). (2022). Venues for Machine Learning&nbsp; Machine Learning for
Social Science. Retrieved from https://ms.pubpub.org/pub/ml

Zhang, L. (Sunshine). (2022). Computing Platforms: Set up the Workspace for Machine
Learning Projects. Machine Learning for Social Science. Retrieved from
https://ms.pubpub.org/pub/computing

Zhang, L. (Sunshine). (2022). Resources for Blockchain Network Studies. Machine Learning for
Social Science. Retrieved from https://ms.pubpub.org/pub/network

