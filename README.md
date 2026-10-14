# insurance-dataset-hierarchical-clustering
Unsupervised customer segmentation and risk analysis on insurance dataset using Hierarchical Agglomerative Clustering and dendrogram visualization.

# Insurance Dataset Customer Segmentation using Hierarchical Clustering

## 1. Business Problem
### 1.1. Business Objective
To group insurance policyholders based on demographic details, coverage types, and claim behaviors using hierarchical clustering. This helps the insurance firm optimize risk assessment, tailor premium offerings, and design targeted retention strategies.
### 1.2. Constraints
* Managing mixed data types and scaling discrepancies between monetary amounts and demographic features.
* Ensuring cluster interpretability for business decision-making.

## 2. Data Dictionary
| Feature Name | Data Type | Description |
| --- | --- | --- |
| `ID` / `Policy_ID` | String/Integer | Unique policyholder identifier |
| `Age` / `Demographics` | Numerical/Categorical | Policyholder age and background details |
| `Coverage_Type` | Categorical | Level of insurance coverage selected |
| `Premium_Amount` | Numerical | Monthly or annual insurance premium paid |
| `Claim_Amount` / `History` | Numerical | Total historical claim payouts |

## 3. Data Pre-processing
* **Data Cleaning:** Handled missing data entries and removed redundant identifier columns.
* **Feature Engineering & Normalization:** Converted categorical fields to dummy variables and applied standard scaling (`StandardScaler`) on numerical metrics.

## 4. Exploratory Data Analysis (EDA)
* **Summary:** Statistical overview of premium distributions and claim histories.
* **Univariate Analysis:** Density plots and boxplots showing the spread of policy amounts.
* **Bivariate Analysis:** Scatter plots illustrating relationships between premiums and claim payouts across groups.

## 5. Model Building
* **5.1 Scaled Data Models:** Developed agglomerative hierarchical clustering models using Euclidean distance and Ward's linkage.
* **5.2 Dendrogram Visualization:** Generated dendrograms to track cluster merges and select the optimal cutoff height.
* **5.3 Cluster Validation & Insights:** Labeled clusters to define clear customer risk segments.

## 6. Business Benefits & Impact
* Enables data-driven underwriting and precision pricing models.
* Enhances profitability by segmenting high-risk versus low-risk policyholders accurately.
