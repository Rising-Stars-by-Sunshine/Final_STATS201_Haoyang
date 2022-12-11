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
| **Queried Data**   |   [Return_Queried](https://github.com/Rising-Stars-by-Sunshine/YutongQuan_STATS201_FinalProject/blob/main/data/Queried_Data)   |                                 -                                |
| **Processed Data** | [Return_Processed](https://github.com/Rising-Stars-by-Sunshine/YutongQuan_STATS201_FinalProject/tree/main/data/Processed_Data) |                                 -                                |

## Code
- [Query Data]()
- [Process Data]()
- [Analyze Data]()

## Spotlight
- **Posters**:

![poster](https://github.com/Rising-Stars-by-Sunshine/Final_STATS201_Haoyang/blob/main/spotlight/Poster.png)
***Figure No.1**. Project Poster (created by [Canva](https://www.canva.com/design/DAFT-dVPBOM/fzR4WbsJPm6xCImV6BYMOA/view?utm_content=DAFT-dVPBOM&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton))*

- **Contribution to the Literature**:

<img src="https://github.com/Rising-Stars-by-Sunshine/Final_STATS201_Haoyang/blob/main/spotlight/Contribution%20to%20the%20Literature.png" height="500" alt="Contribution to Literature"/><br/>
***Figure No.2**. Contribution to the Literature (created by [Whimsical](https://whimsical.com))*

<img src="https://github.com/Rising-Stars-by-Sunshine/Final_STATS201_Haoyang/blob/main/spotlight/Spillover17-21.png" height="300" alt="Spillover of portfolios from 2021-2022"/><br/>
***Figure No.3**. Spillover of portfolios from 2021-2022. For the defensive strategy, it is 53.6–52.5 = 1.1 percent, for the ESG strategy, it is 59.7–54.1 = 5.6 percent, and for the EAFE strategy, it is 44.3–37.7 = 6.6 percent. In general, the capital flows away from the defensive and ESG portfolios to the EAFE portfolio.
