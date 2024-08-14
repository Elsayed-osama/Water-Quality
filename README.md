# Water Quality Analysis

## Overview

Access to safe drinking water is a fundamental human right and a cornerstone of public health. Investments in water supply and sanitation often provide significant economic benefits by reducing health risks and healthcare costs. This repository contains an analysis of water quality metrics to assess the potability of various water sources.

## Dataset

The dataset `water_potability.csv` includes water quality metrics for 3,276 different water bodies. The key parameters are as follows:

1. **pH Value**: Measures the acid-base balance of water. WHO recommends a pH range from 6.5 to 8.5. The values in this dataset range from 6.52 to 6.83, which are within WHO standards.

2. **Hardness**: Indicates the concentration of calcium and magnesium salts in water. Hardness affects the water's ability to precipitate soap and is influenced by the water's contact with geological deposits.

3. **Total Dissolved Solids (TDS)**: Reflects the concentration of dissolved minerals and salts in water. High TDS values indicate high mineralization. The desirable limit for TDS is 500 mg/L, with a maximum limit of 1000 mg/L for drinking purposes.

4. **Chloramines**: Disinfectants used in public water systems, formed by adding ammonia to chlorine. Safe levels are up to 4 mg/L.

5. **Sulfate**: Naturally occurring in minerals, soil, and water. Sulfate concentrations range from 3 to 30 mg/L in most freshwater supplies, though some areas may have concentrations up to 1000 mg/L.

6. **Conductivity**: Measures the water's ability to conduct electricity, which correlates with ion concentration. WHO recommends an EC value not exceeding 400 μS/cm.

7. **Organic Carbon**: Measures the total carbon in organic compounds in water. US EPA standards recommend less than 2 mg/L in treated water and less than 4 mg/L in source water.

8. **Trihalomethanes (THMs)**: Chemicals that may form when chlorine is used to treat water. Safe levels are up to 80 ppm.

9. **Turbidity**: Indicates the amount of solid matter in suspension. The mean turbidity value for Wondo Genet Campus is 0.98 NTU, below the WHO recommended maximum of 5.00 NTU.

10. **Potability**: Indicates if water is safe for human consumption, with 1 meaning potable and 0 meaning not potable.

## Analysis and Models

The dataset has been subjected to Exploratory Data Analysis (EDA) and visualization to uncover insights into water quality. Data preprocessing was performed to address class imbalances. Four machine learning models were applied:

1. **Support Vector Classifier (SVC)**
2. **K-Nearest Neighbors (KNN)**
3. **Decision Tree Classifier**
4. **Random Forest Classifier**

The **Random Forest Classifier** achieved the highest accuracy in predicting water potability.

## Usage

To replicate or extend the analysis:

1. Clone the repository: `git clone https://github.com/your-username/your-repository.git`
2. Navigate to the project directory.
3. Install required packages: `pip install -r requirements.txt`
4. Run the analysis script: `python analysis.py`

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

Special thanks to data contributors and organizations working towards improving water quality and accessibility.
