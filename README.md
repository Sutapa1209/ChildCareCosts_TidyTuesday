## ChildCareCosts_TidyTuesday
Welcome!

## Aim of the Analysis

  The goal of this project was to explore trends and predictors of childcare costs in the United States using the TidyTuesday Childcare dataset. 
  Key areas of focus included:
- Examining national trends in childcare costs and median household income across U.S. counties (2008–2018)
- Conducting descriptive analyses of gender-based differences in median earnings, occupational categories, racial/ethnic composition, and household family structures
- Using visualizations (plots, maps) and multilevel regression models to investigate:
         - How gender dynamics in labor force participation rates (LFPR) influence infant childcare costs
         - The geographical distribution of infant childcare costs across U.S. states by age group
         - Differences in childcare costs by child age group (infant, toddler, preschool)
         - Racial/ethnic disparities in childcare costs
…etc. 

## How to Run

This analysis is provided in a Jupyter Notebook (`ChildCare_TidyTuesday.ipynb`).

### To run the code:
1. Open the notebook in any Jupyter-compatible environment, such as:
   - Jupyter Notebook
   - JupyterLab
   - VS Code with the Jupyter extension
   - Google Colab

2. Run each cell in order, from top to bottom.

> Note: If using Google Colab, you can upload the notebook directly and run it in-browser without installing anything.


## Dependencies
Ensure the following packages are installed:

```r
install.packages(c(
  "tidyverse",
  "maps",
  "ggplot2",
  "dplyr",
  "scales",
  "patchwork",
  "ggpubr",
  "tidyr",
  "RcppEigen",
  "lme4",
  "pbkrtest",
  "car",
  "rstatix",
  "corrplot"
))
```


## Summary of Results

> Income and Childcare Costs:
 - Descriptive analysis confirmed a clear positive relationship between income and childcare expenses, i.e. counties with higher median household income tend to have higher weekly infant care costs,
 - Interestingly, even though median income dropped during the Great Recession (around 2008–2010), childcare costs for infants, toddlers, and preschoolers continued to rise steadily across all age groups.
- This divergence highlights a growing burden of childcare affordability, placing greater financial strain on families with young children.

>Types of Childcare:
- Center-based care remains consistently more expensive compared to family-based childcare with all age groups 
- Childcare for all 3 age groups- infant, toddler, and preschool steadily increased over time (2008-2018)
- Infant care remains consistently costlier followed by Toddler, and preschool being the cheapest. 

> Regional Inequities: 
-  A clear regional divide emerges, with Midwestern and Southern states generally showing lower costs across all care types. Western and Northeastern states consistently appear more       expensive regardless of age group.

> Labor Force Participation and Childcare Costs
- There is a significant relationship between labor force participation rate (LFPR) and infant care costs, and this relationship differs by gender.
- Specifically, counties with higher female LFPR are associated with sharper increases in infant care costs than counties with higher male LFPR.
- Thus, this shows infant care markets may be more responsive to women’s labor force participation (who traditionally bear more caregiving responsibilities), than males.
- Moreover, counties with higher female LFPR clustered in regions with both higher income and higher childcare costs.
- This suggests that growing female workforce participation, especially in wealthier regions, may reflect increased need for formal childcare—underscoring the importance of expanding affordable care infrastructure to meet rising demand.

..other demographic-based descriptive analyses were carried out showing gender-based differences in occupational categories, 
Composition of various family structures (both parents working, only father working, only mother working, etc.), racial/ethnic composition, etc. 

## 📁 File Structure

- `ChildCare_TidyTuesday.ipynb`: Full code for data analysis and visualizations  
- `README.md`: This file  
- `figures/`: Folder containing generated plots (optional)

