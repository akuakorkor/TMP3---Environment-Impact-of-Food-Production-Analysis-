# TMP3---Environment-Impact-of-Food-Production-Analysis-

## 1. Business Understanding

**Project Objective**
This project aims to evaluate the environmental footprint of food production, focusing on carbon emissions, water consumption, and land use. The analysis offers data-driven insights to reduce environmental degradation and promote sustainable food systems, supporting policymakers, producers, and consumers alike.

**Primary Goals:**

* Analyze the environmental impact of different food products based on:

1. Carbon emissions

2. Water usage

3. Land use

* Identify and compare high-impact and low-impact foods.

* Offer actionable, data-based recommendations for more sustainable food production and consumption.

### 📌 Analytical Questions
- Which food items emit the most and least carbon?
- How does environmental impact compare between plant-based and animal-based foods?
- What correlations exist between land use, water use, and emissions?
- Which production stages (e.g., farm, transport, packaging, retail) have the highest emissions?
- What environmental impact do different food types (cereals, dairy, meat, vegetables) have?
- What are the key contributors to eutrophication (nutrient pollution in water)?
- Can clustering techniques group foods by environmental impact?

### 📌 Hypothesis Testing
- **H₀ (Null Hypothesis):** No significant difference in environmental impact between plant-based and animal-based foods.
- **H₁ (Alternative Hypothesis):** Animal-based foods have a significantly higher environmental impact than plant-based foods.

**Hypothesis Testing Summary**

| Metric            | U-statistic | p-value | Result                    |
|-------------------|-------------|---------|---------------------------|
| Total Emissions   | 27.0000     | 1.0000  | No significant difference |
| Total Water Use   | 91.0000     | 0.9840  | No significant difference |
| Total Land Use    | 59.0000     | 0.9989  | No significant difference |

---

## 2. Data Understanding

The dataset includes 43 food products with 23 features detailing environmental impacts such as greenhouse gas emissions, land use, and water use across production stages.

**Key Features:**
- Emissions across stages (land use change, animal feed, transport, packaging, etc.)
- Eutrophication (nutrient runoff into water bodies)
- Metrics on land and water usage
- Stage-wise emission breakdown (farm, transport, packaging, retail)

**EDA Insights:**
- Most features are right-skewed.
- High-impact outliers detected in land use and farm emissions.
- PCA revealed that most variance is captured in the first component (PC1).

---

## 3. Data Preparation

**Handling Missing Values:**
- No significant missing data due to small dataset size.
- Column names were standardized to fix inconsistencies.

**Feature Engineering:**
- Added features like food categories and Total Environmental Impact by aggregating normalized metrics.
- Missing values filled using Median to avoid outlier bias.

**Data Quality:**
- Corrected misspelled column "Packging" to "Packaging".

---

## 4. Modeling

**Clustering (K-Means & Hierarchical):**
- Grouped food items based on Plant-Based and Animal-Based categories.

**Correlation Analysis:**
- Measured relationships between land use, water use, and emissions.
- Found strong correlation between land use and emissions.

**Hypothesis Testing:**
- Applied Mann-Whitney U test to compare plant- vs animal-based food impacts.
- Found no significant differences.

**PCA (Principal Component Analysis):**
- Reduced feature dimensions while preserving variance.
- Highlighted key variables influencing environmental impact.

---

## 5. Evaluation

### 📌 Key Findings
- Animal-based foods emit more greenhouse gases, but plant-based items still impact water and land use.
- Farm and land-use change are the largest contributors to environmental impact.
- High-impact foods: beef, lamb, cheese
- Low-impact foods: peas, nuts, soy
- Clustering revealed distinct food groups, aiding in prioritizing sustainability efforts.

### 📌 Limitations
- Source data accuracy may vary.
- Socio-economic aspects (e.g., accessibility, affordability) not included.

---

## 6. Recommendations

### 📌 Sustainability Recommendations

**Policy & Regulation:**
- Implement carbon taxes on high-impact products.
- Promote research into eco-friendly farming techniques.

**Consumer Awareness:**
- Encourage plant-based food choices.
- Label products with environmental impact scores.

**Industry Innovations:**
- Use smarter farming to reduce land use.
- Streamline supply chains to reduce emissions.
- Innovate sustainable packaging solutions.

### 📌 Future Work
- Include real-time emissions tracking.
- Apply ML for predictive modeling of food impacts.

---

## 7. Deployment
[View Power BI Dashboard](https://app.powerbi.com/links/nGU_G564I8?ctid=7bfb1286-b735-4395-8ea0-ed2c4861d742&pbi_source=linkShare)

[Published Article](https://medium.com/@akuaakonnor43/foodprint-insights-a-four-week-data-science-journey-c9ec5340ecc5)
---

## 8. Conclusion
This project provides in-depth analysis of food production’s environmental footprint and offers evidence-based recommendations to improve sustainability. Using clustering, PCA, and hypothesis testing, the study highlights high-impact foods and presents paths toward a more sustainable food system.
