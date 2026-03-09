# Project-Udaan

# Identifying Hidden Health-Food Consumers in Non-Metro India (Excel Analytics Project)

## Project Overview

This project analyzes household consumption data to identify potential consumers of healthy packaged breakfast products such as oats and muesli in non-metro regions of India.

The objective is to move beyond traditional income-based segmentation and instead identify **emerging middle-class households with strong purchasing power and modern consumption behavior**.

The analysis focuses on detecting **high purchasing power households that are not yet buying oats**, representing an untapped market opportunity.

---

## Business Problem

Many FMCG companies assume that premium health food products are mainly consumed by **urban, high-income households**. However, consumption patterns are changing in India.

The challenge is to identify:

* Hidden affluent households in Tier-2 and rural regions
* Consumers with modern lifestyles and health awareness
* Districts with strong potential for expanding healthy breakfast products

---

## Dataset Description

The dataset contains household-level consumption data including:

* Household assets (cars, AC, appliances)
* Monthly expenditure across various categories
* Income information
* Geographic identifiers (districts and region types)

### Data Cleaning Assumption

The dataset contained "-99" values representing unavailable data.
For simplification, all  "-99" values and missing values were treated as  "0" during preprocessing.

---

## Tools Used

* Microsoft Excel (Advanced Excel)
* Pivot Tables
* Data Cleaning Techniques
* Feature Engineering
* Exploratory Data Analysis
* Dashboard Visualization

---

## Methodology

### 1. Data Cleaning

* Converted `-99` and blank values to `0`
* Standardized expenditure columns

### 2. Target Variable Creation

Created a binary variable:

OATS_BUYER

* `1` → household purchases oats/muesli
* `0` → household does not purchase oats

---

### 3. Purchasing Power Index (PPI)

Since income can be unreliable in informal economies, purchasing power was estimated using:

**Asset Ownership**

* Cars
* AC
* Refrigerator
* Washing Machine
* Computers
* Houses

**Lifestyle Spending**

* Restaurants
* Gym/Fitness
* OTT Streaming
* Ready-to-eat foods
* Bottled water

PPI Formula:

PPI = Asset Score + Lifestyle Score

---

### 4. High Purchasing Power Identification

Top **30% of households by PPI** were classified as **High Purchasing Power households** using percentile analysis.

---

### 5. Hidden Affluent Segment

Households with:

* **Low reported income**
* **High Purchasing Power Index**

were classified as **Hidden Affluent Consumers**.

These households demonstrate strong consumption patterns despite lower reported income.

---

### 6. Market Penetration Analysis

Calculated the percentage of households currently purchasing oats to understand market penetration.

---

### 7. Consumer Behavior Analysis

Compared spending patterns of:

* Oats buyers
* Non-buyers

Key categories analyzed:

* Gym/Fitness
* Restaurants
* Ready-to-eat foods
* Bottled water
* Health supplements

---

### 8. District-Level Opportunity Analysis

Pivot tables were used to identify districts with:

* High purchasing power
* Higher oats consumption
* Strong potential demand

Top districts represent **pilot markets for expansion**.

---

## Dashboard Visualizations

The Excel dashboard includes:

1. **Market Penetration Chart**

   * Oats Buyers vs Non-Buyers

2. **Top Districts for Oats Consumption**

   * Average spending on oats by district

3. **Lifestyle Spending Comparison**

   * Spending behavior of buyers vs non-buyers

4. **Oats Adoption by Asset Ownership**

   * Relationship between wealth indicators and product adoption

---

## Key Insights

* Income alone is not a reliable indicator of purchasing power.
* Asset ownership and lifestyle spending provide a stronger signal of consumption capability.
* A **Hidden Affluent segment exists in Tier-2 and rural markets**.
* Health-conscious households show significantly higher spending on:

  * Fitness
  * Restaurants
  * Ready-to-eat foods
* Several non-metro districts demonstrate strong potential for healthy packaged breakfast products.

---

## Business Recommendations

1. Expand product availability in **Tier-2 markets and emerging districts**
2. Partner with **modern kirana stores and pharmacies**
3. Promote products through **gym partnerships and health-focused marketing**
4. Use **digital advertising targeting lifestyle and health-conscious consumers**

---

## Project Outcome

This analysis demonstrates how data-driven consumer segmentation can reveal **hidden demand in non-metro markets**, enabling FMCG companies to expand beyond traditional urban markets.

---

## Author

Vineet Gupta
Aspiring Business / Data Analyst

Skills demonstrated:

* Data Cleaning
* Consumer Segmentation
* Business Analytics
* Dashboard Development
* Market Opportunity Analysis
