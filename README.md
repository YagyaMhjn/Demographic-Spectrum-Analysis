# Beyond the Diagnosis: A Demographic and Behavioral Profiling of Autism Spectrum Traits

## Overview

This project presents a comprehensive **Exploratory Data Analysis (EDA)** of Autism Spectrum Disorder (ASD) screening data. It focuses on uncovering how behavioral traits and demographic factors interact, moving beyond binary diagnosis to provide deeper insights into ASD patterns.

The analysis emphasizes **behavioral profiling, demographic segmentation, and risk factor assessment** using a structured data analytics pipeline.

---

## Problem Statement

Autism Spectrum Disorder (ASD) manifests through diverse behavioral and social interaction patterns. Traditional diagnosis often simplifies this complexity into binary outcomes.

This project addresses the need to:

* Understand **variation in ASD traits across demographics**
* Identify **behavioral patterns and clusters**
* Evaluate **medical and genetic risk factors**
* Reveal **hidden insights beyond diagnosis labels**

---

## Objectives

* Analyze ASD traits across **age, gender, and medical history**
* Identify **behavioral clusters and archetypes**
* Evaluate impact of **jaundice and family ASD history**
* Build **composite behavioral scoring systems**
* Generate **actionable insights for research and intervention**

---

## Project Vision

To build an **end-to-end analytical pipeline** that transforms raw screening data into meaningful insights, enabling:

* Better understanding of ASD manifestation
* Identification of high-risk groups
* Data-driven decision-making for clinicians and researchers

---

## Tech Stack

* **Python**
* **Pandas, NumPy**
* **Matplotlib, Seaborn**
* **Missingno**

---

## Dataset Details

* **Records:** 6,075 individuals
* **Original Features:** 15 → Expanded to 26+ after engineering
* **Data Type:** Cross-sectional screening data

### Key Characteristics

* **Gender:** 57.8% Male, 42.2% Female
* **Age Range:** 1–68 years (Mean: 19.84)
* **ASD Positive Cases:** 29.7%

### Risk Factors

* Jaundice: 17.2%
* Family ASD History: 18.5%
* High-Risk (Both): 4.4%

---

## Methodology

1. Data loading and integration
2. Data profiling and validation
3. Cleaning and standardization
4. Feature engineering
5. Risk factor analysis
6. Exploratory data analysis

---

## Feature Engineering

### Behavioral Features (A1–A10)

Binary indicators representing:

* Eye contact
* Communication ability
* Social behavior
* Attention patterns

---

### Composite Scores

#### Social Interaction Score

Measures eye contact and joint attention:

```
A1 + A2 + A6
```

#### Communication Deficit Score

Inverse scoring for communication ability:

```
(1 - A3) + (1 - A4) + (1 - A9)
```

#### Behavioral Atypicality Score

Captures atypical behavioral traits:

```
(1 - A5) + (1 - A7) + (1 - A8) + A10
```

#### Total Atypical Trait Burden

Global severity metric:

```
9 - (A1 + ... + A9) + A10
```

---

## Advanced Features

### Behavioral Archetypes

* Severe Global Delay
* Communication Impaired
* Socially Withdrawn
* Highly Atypical Presentation
* Mild/Typical Presentation

### Clinical Profiles

* Global Cognitive/Emotional Deficit
* Isolated Emotional Deficit
* Other

### Healthcare Flags

* **Late Diagnosis Flag**
* **Masking Proxy Flag**

---

## Key Insights

### 1. Gender Differences

* Females show a higher ASD diagnosis rate (31.7%) vs males (28.2%)

### 2. Risk Amplification

* Highest risk group: **Females with family ASD history (42.7%)**

### 3. Age Patterns

* Diagnosis peaks in:

  * Early childhood
  * Young adulthood

### 4. Behavioral Complexity

* 62.58% of individuals with *mild/typical presentation* were still diagnosed
  → Indicates diagnosis is not purely behavior-score driven

---

## Results Summary

* Successfully engineered **26+ analytical features**
* Identified **distinct behavioral clusters**
* Built **multi-dimensional ASD profiling system**
* Highlighted **non-obvious diagnostic patterns**

---

## Future Work

* Statistical testing (Chi-square, correlation analysis)
* Interactive dashboards
* Real-time filtering of demographic and behavioral data
* Predictive modeling for ASD risk

---

## Contributors

* Yagya Mahajan 
* Arnav Jain

---
