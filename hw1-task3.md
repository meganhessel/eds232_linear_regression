# Homework 1 Task 3

---

Answer the following questions based on exercises from *An Introduction to Statistical Learning with Applications in Python*.

## Chapter 2.4 Exercises

---

### Exercise 1 (ISLP exercise 2)

Explain whether each scenario is a **classification or regression** problem, and indicate whether we are most interested in **inference or prediction**. Finally, provide **n** (size of observation dataset) and **p** (number of predictors).

**(a)**  We collect data on 200 protected marine reserves worldwide. For each reserve we record species richness, reserve size, years since establishment, enforcement budget, and proximity to human settlements. We are interested in understanding which factors affect species richness.

The goal is to understand which predictors are associated with the response (species richness). Thus, they are interested in **inference**.
The scenario is a **regression** problem since the vairables are numeric and continous. 
There are **4** predictors: reserve size, years since establishment, enforcement budget, and proximenty to human settlement. 
n = **200** as they collected data on protected marine reserves. 

---

**(b)** A conservation agency wants to know whether a proposed habitat corridor will successfully support wildlife movement or fail to do so. They collect data on 30 previously established corridors. For each corridor they have recorded whether wildlife movement was successful or unsuccessful, corridor width, length, surrounding land use type, and eight other variables.

The goal is to predict the impact of a habitate coordidor . Thus, they are interested in **prediction** 
The scenario is a **classification** problem since the response is successful vs unsuccessful (discrete categorical labels).  
There are **11** predictors: coordor width + length, land use type, and 8 more. 
n = **30** as there are 30 studied corridors. 

---

**(c)** We are interested in predicting weekly average ground-level ozone concentration in a coastal city. We collect weekly data for all of 2019. For each week we record average ozone concentration, sea surface temperature, wind speed, solar radiation, and atmospheric

The goal is to predict weekly average ground-level ozone concentrations. Thus, they are interested in **prediction**. 
The scenario is a **regression** problem since they are studying countinous numeric ozone concentrations. 
There are **4** predictors: sea surface temperature, wind speed, solar rasiation, and atmospheric. 
**n = 52** as there is data for each week of 2019. 

---

### Exercise 2 (ISLP exercise 5)

What are the advantages and disadvantages of a very flexible (versus a a less flexible) approach for regression? Under what circumstances might a more flexible approach be preferred to a less flexible approach? When might a less flexible approach be preferred?

**Flexible Regession:**
-  Pros: Can capture complex/non linear/high-dimensional trends; Decrease bias (underfitting). 
-  Cons: High variance (overfitting); Can be difficult to interpret. 
-  Perferred: Large dataset; Goal is prediction. 

**Less flexible Regression:**
-  Pros: Simple to interpret; Less susceptable to noise.
-  Cons: High bias (if relationship is not linear); Cannot capture complex patterns.
-  Perferred: Small dataset; When relationship is linear.
 
---

### Exercise 3 (ISLP exercise 6)

Describe the differences between a **parametric** and a **non-parametric** statistical learning approach. What are the **advantages** of a parametric approach to regression or classification (as opposed to a non-parametric approach)? What are its **disadvantages**?

**Parametric:**
-  Data assumes a specific distrubution (typically normal distribution).
-  Pros: Higher statistical power when assumptions are met. 
-  Cons: Stringent assumptions (AKA assumption must be met); Sensitive to outliars.
-  Examples: T-test, ANOVA, Linear regression 

**Non-Parametric:**
-  No assumptions about data's distribution. 
-  Pros: More robust - used with skewed and not normal data. 
-  Cons: Lower statistical power. 
-  Examples: Mann-Whitney U, Kruskal-Wallis, Wilcoxon