# Choice Experiment on Alternative Food-Away-From-Home Outlets

**Author:** Suraj Gurung  
**Last Updated:** October 8, 2024  
**Tools:** R  

---

## 📌 Project Overview

This project examines consumer preferences for emerging food-away-from-home outlets within the **Home Cooking Movement (HCM)**. Using a stated **discrete choice experiment**, the analysis estimates how consumers value:

- Regulatory oversight  
- Food safety certifications  
- Customer reviews  
- Liability insurance signals  
- Pricing levels  

The results provide evidence for:
- Market entry strategies for food entrepreneurs  
- Pricing decisions and trust-building  
- Local food safety policy and certification frameworks  

---

## 📁 Project Files

| File Name | Description |
|-----------|-------------|
| **`DesignofExperiment.Rmd`** | Creates a D-efficient fractional factorial design for the choice experiment, including attribute level coding, blocking, and priors. |
| **`HCM.Rmd`** | Performs data cleaning, descriptive analysis, and estimation of Conditional Logit and Mixed Logit models to derive consumer willingness-to-pay (WTP) estimates. |

---

## 📊 Methods & Statistical Models

### **Experimental Design**
- Fractional factorial choice design  
- D-efficiency optimization  
- Bayesian priors for parameter stability  
- Blocking & constraint checks  

### **Discrete Choice Modeling**
- Mixed Logit (RPL/RP Logit) using `gmnl`   
- WTP estimation via simulated maximum likelihood  
- Attribute interactions and segmentation insights  

---

## ⚙️ Required R Packages

```r
library(mlogit)
library(idefix)
library(AlgDesign)
library(tidyverse)
library(gmnl)   # for Mixed Logit (older version may be required)
