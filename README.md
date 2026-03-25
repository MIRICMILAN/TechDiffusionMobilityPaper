# Technology Diffusion, Human Capital, and Employee Mobility

**Authors:** Milan Miric (University of Southern California) and Hakan Ozalp (University of Amsterdam)

## Abstract

As new technologies diffuse within an industry, they impact the value of worker skills, and in turn may influence the mobility of workers between firms in that industry. This mobility may be particularly pronounced for individuals whose jobs are complementary to these new technologies and therefore increases demand for these individuals. In this paper, we investigate the impact of a small set of development tools diffusing within an industry and investigate whether this was associated with an increase in worker mobility for individuals with complementary skills, compared to those with (partly) substitutable ones. Specifically, we study the diffusion of middleware tools within the video game industry that made human capital more general by making it industry-specific (rather than firm-specific), and was complementary to the tasks being performed by Creatives in this industry, compared to Programmers. We exploit the uneven diffusion of these tools across genres to investigate whether workers experienced greater mobility in the genre where the technologies diffused more broadly. We also find greater mobility between projects that used the same middleware components. We find that the diffusion of these tools was associated with greater mobility for creatives than for programmers. These results are robust to a variety of empirical checks and speak to the impact of broad diffusion of IT tools, which may enable workers to more easily move between companies.

## Transparency Materials

This repository contains the **transparency materials** for the paper. These materials include the Stata do-files and Jupyter Notebooks necessary to replicate the analysis and figures presented in the study.

**Note on Data Availability:** The dataset used to perform this analysis included data on product sales which was licensed and cannot be publicly shared. The dataset with the publicly availible data will be made availible. 

## Table of Contents

* **[Figures & Tables/](./Figures%20&%20Tables)**
    * `Table 1.html`: Baseline regression results (Full Sample, Creatives, Programmers).
    * `Table 2.html`: Results using the alternative "Popular Middleware" definition.
    * `Table 3.html`: Results using the Share-Based diffusion measure.
    * `Middleware_Share_Over_Time.png`: Figure showing the diffusion of any third-party middleware over time.
    * `Popular_Middleware_Share_Over_Time.png`: Figure showing the diffusion of popular middleware over time.
    * `Middleware_Usage_By_Genre.png`: Breakdown of middleware usage by game genre.
    * `Margins Plot - Likelihood of Changing Employer by Genre and Middleware (Full Sample).png`: Marginal effects plot for the full sample.
    * `Margins Plot - Likelihood of Changing Employer by Genre and Middleware (Programmers and Creatives).png`: Marginal effects plot stratified by role.
    * `Margins Plot - Likelihood of Changing Employer Post Middleware By Previous MIddleware Use.png`: Cross-sectional mobility differences in the post-adoption period.
    * `Coefplot_Popular_Middleware.png`: Coefficient plot of mobility trends using popular middleware.
    * `Coefplot_Any_Middleware.png`: Coefficient plot of mobility trends using any middleware.
    * `Baseline_Mobility_Trends.png`: Baseline probability of changing employers over time.

* **[Scripts/]**
    * `Dataset Construction & Regression Analysis.ipynb`: The primary notebook that performs data cleaning, merges datasets, runs Stata regressions, and generates the regression tables and marginal effects plots.
    * `Descriptive Figures.ipynb`: Python notebook used to generate the descriptive diffusion and genre breakdown figures.

## Summary of Results

This study examines how the diffusion of middleware technology in the video game industry affects the mobility of high-skilled workers. We find that the adoption of middleware is associated with distinct mobility patterns for different types of human capital.

### 1. Technology Diffusion
Middleware usage increased significantly during the sample period, particularly after 2002. The figure below illustrates the rising share of game titles utilizing third-party middleware components.

<img src="./Figures%20&%20Tables/Middleware_Share_Over_Time.png" width="600" />

### 2. Mobility Patterns
Our baseline regression analysis reveals a differential impact on worker mobility based on their role. The marginal effects plots below show the predicted likelihood of a worker changing employers, comparing those who worked on projects with middleware versus those who did not, stratified by game genre (Shooter vs. Non-Shooter).

**Programmers vs. Creatives**
For **Programmers** (lower panels), working with middleware is associated with a lower likelihood of mobility, consistent with the standardization of technical skills. Conversely, for **Creatives** (upper panels), middleware usage is associated with higher mobility, suggesting that these tools allow their specialized artistic skills to be more easily transferred across firms.

<img src="./Figures%20&%20Tables/Margins%20Plot%20-%20Likelihood%20of%20Changing%20Employer%20by%20Genre%20and%20Middleware%20(Programmers%20and%20Creatives).png" width="600" />

For a complete discussion of the methodology and results, please refer to the full paper.
