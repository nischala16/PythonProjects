# Pinterest Shop the Look — Fashion Dataset Analysis

## Overview

This repository contains a comprehensive exploratory data analysis (EDA) of the **Pinterest Shop the Look** fashion dataset. The dataset includes scene-product pairs with bounding box locations and product category information. This project aims to understand the data structure, explore key patterns, and generate insights that can inform downstream tasks such as recommendation systems and machine learning models.

---

## Project Structure

- `fashion-project/`  
  - `0_data_load_and_eda.ipynb` — Initial data loading and detailed exploratory data analysis of the fashion dataset. Includes summary statistics, visualizations of product categories, bounding box sizes, scene complexity, and correlations.  
  - `fashion.json` — Raw scene-product pair data for fashion.  
  - `fashion-cat.json` — Product category mappings for the fashion dataset.  

*Future notebooks and scripts for machine learning models, recommendation systems, and advanced analysis will be added here.*

---

## Dataset Description

- **Source:** [Pinterest Shop the Look Dataset](https://github.com/wckang/Shop-the-Look-Dataset)  
- **Content:** The dataset consists of images from Pinterest, annotated with bounding boxes that identify products within scene images. Each product is associated with a category label.  
- **Key Columns:**  
  - `product` — Unique product ID  
  - `scene` — Unique scene ID  
  - `bbox` — Bounding box coordinates (left, top, right, bottom) normalized between 0 and 1  
  - `category` — Product category label  

---

## Exploratory Data Analysis Highlights

- Dataset contains over 72,000 bounding boxes across ~38,000 unique products and ~29,000 unique scenes.  
- Product categories are distributed unevenly, with some categories (e.g., Apparel & Accessories) dominating the dataset.  
- Bounding box size analysis shows variation in product scale across categories.  
- Scenes contain a varying number of products, indicating differing scene complexity.  
- Correlation analysis reveals moderate positive correlation between bounding box width and height.  

Visualizations include bar charts of top product categories, boxplots of bounding box dimensions by category, histograms of products per scene, and heatmaps of product-scene interactions.

---

## How to Use

1. Clone this repository.  
2. Launch the Jupyter notebook `0_data_load_and_eda.ipynb` to explore the initial data analysis.  
3. Follow the notebook markdown and comments for detailed explanations of each step.  
4. New notebooks with machine learning models and recommendation system implementations will be added in the near future to extend this analysis.

---

## Requirements

- Python 3.x  
- Jupyter Notebook  
- Packages: `pandas`, `numpy`, `matplotlib`, `seaborn`, `jsonlines`

## Next Steps
Build recommendation models to predict complementary products based on scene context.

Implement machine learning workflows to enhance product detection and category prediction.

Extend analysis to the home dataset (home.json, home-cat.json).

Explore image-based features and deep learning for improved recommendations.

## References
Wang-Cheng Kang et al. "Complete the Look: Scene-based Complementary Product Recommendation." CVPR 2019.

Dataset source: https://github.com/wckang/Shop-the-Look-Dataset



