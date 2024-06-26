# Recommendation-System-for-purchase-at-Zepto

## Project:

The project involves implementing a recommendation system for purchase at Zepto, an e- commerce platform, to enhance user experience and drive sales. The goal is to leverage user
behavior data and machine learning algorithms to deliver personalized product recommendations tailored to individual preferences.

## Analysis:
Extensive analysis was conducted on user interactions, including browsing history, purchase patterns, and feedback, to understand customer preferences and behavior. This was done by
circulating google forms to the respondents and then making use of Association rules using R 4.4.0 software. The analysis part is explained in detail in later part.

## INTRODUCTION TO BUSINESS

### a) Introduction to Zepto:
Zepto is a dynamic e-commerce platform founded in 2021. Owned and operated by two Stanford University drop-outs Aadit Palicha and Kaivalya Vohra, it has emerged as a leading player in the online retail space. With a commitment to
innovation and customer satisfaction, Zepto offers a diverse range of products and services tailored to meet the evolving needs of its global customer base. The company's ownership structure reflects a blend of strategic investors, venture
capitalists, and individual stakeholders, all united by a shared vision of driving growth and excellence in the digital marketplace.


<img width="355" alt="image" src="https://github.com/dhanashreehampiholi/Recommendation-System-for-purchase-at-Zepto/assets/57892263/123e400b-1768-4370-b361-00d2af12ad6c">


### b) Introduction to Products Sold and Pricing Range:
Zepto caters to a wide array of consumer needs, offering an extensive selection of products spanning categories such as electronics, fashion, home goods, beauty, and
more. From affordable essentials to premium brands, Zepto ensures there's something for every budget and preference. With competitive pricing and frequent
promotions, customers enjoy access to quality products at compelling prices. Whether shopping for everyday essentials or indulging in luxury items, Zepto
delivers a seamless and rewarding shopping experience.


<img width="161" alt="image" src="https://github.com/dhanashreehampiholi/Recommendation-System-for-purchase-at-Zepto/assets/57892263/dfef0c2a-431c-4c19-a56a-3dd23b75e140">


### c) Introduction to Customer Profile Visiting the Business:
At Zepto, customer satisfaction is paramount, and the diverse clientele reflects this commitment. From tech-savvy millennials seeking the latest gadgets to discerning
professionals in search of stylish apparel, Zepto caters to a broad demographic spectrum. Families, students, and working professionals alike find value in Zepto's
offerings, drawn by the convenience, affordability, and quality synonymous with the brand. With a focus on delivering personalized service and exceeding customer
expectations, Zepto continues to attract and serve a loyal and ever-expanding customer base.


<img width="249" alt="image" src="https://github.com/dhanashreehampiholi/Recommendation-System-for-purchase-at-Zepto/assets/57892263/8bbed424-4739-4cfe-af8f-54db48ff9253">

## INTRODUCTION TO DATA COLLECTION AND DATA METHODOLOGY

### 1. Introduction to Association Rules

Association rules are a fundamental concept in data mining and machine learning, used to discover interesting relationships or patterns in large datasets. The concept is often
applied in market basket analysis, where the goal is to identify associations between products that are frequently purchased together. In association rule mining, a dataset is typically represented as a transaction database,
where each transaction contains a set of items. The goal is to find rules of the form {A} -> {B}, which indicates that if item A is purchased, then item B is also likely to be
purchased.

There are several key components in association rule mining:

Support: The support of a rule {A} -> {B} is the proportion of transactions in the dataset that contain both A and B. It is calculated as the number of transactions containing both
A and B divided by the total number of transactions. 

Confidence: The confidence of a rule {A} -> {B} is the proportion of transactions that contain A which also contain B. It is calculated as the number of transactions containing
both A and B divided by the number of transactions containing A.

Lift: The lift of a rule {A} -> {B} measures how much more likely item B is to be purchased when item A is purchased, compared to when item B is purchased regardless
of A. It is calculated as the confidence of the rule divided by the support of B.

Association rule mining is widely used in retail and e-commerce for market basket analysis, where it helps retailers understand customer purchasing patterns and optimize
product placement, promotions, and cross-selling strategies. It is also used in other domains such as healthcare, telecommunications, and bioinformatics for various data
analysis tasks.


### 2. Introduction to relevance of Association Rules in the context of the project.

Relevance of Association Rules in Zepto’s Recommendation System In Zepto's recommendation system, association rules play a crucial role in enhancing the accuracy and relevance of product recommendations. Association rules mining, a
technique used in data mining and machine learning, helps identify patterns and relationships among items frequently purchased together by users. Here's how association
rules are relevant to Zepto's recommendation system:

#### 1. Identifying Product Associations:

Association rules analysis helps Zepto identify products that are frequently purchased together or have a strong correlation in user behavior. For example, if many users who purchase smartphones also buy phone cases
and screen protectors, the recommendation system can leverage these associations to suggest complementary products to users browsing smartphones.

#### 2. Cross-Selling and Upselling Opportunities: 

By understanding product associations, Zepto can effectively cross-sell and upsell relevant items to customers. For instance, if a user adds a laptop to their cart, the recommendation system can suggest accessories such as
laptop bags, mice, or software, increasing the likelihood of additional purchases and boosting sales revenue.

#### 3. Enhancing Personalization: 

Association rules allow Zepto to personalize recommendations based on individual user behavior and preferences. By analyzing past purchase patterns and item associations specific to each user, the recommendation system
can generate personalized suggestions that align with the user's interests and needs, leading to a more engaging shopping experience.

#### 4. Improving Recommendation Diversity: 
Association rules help diversify product recommendations by suggesting items that are not only related to the user's current selection but also complementary or alternative choices. This ensures that users are
exposed to a broader range of products, reducing the risk of recommendation fatigue and enhancing user satisfaction.


Overall, association rules mining adds a layer of intelligence to Zepto's recommendation system, enabling it to deliver more accurate, relevant, and personalized product
suggestions to users, ultimately driving engagement, conversion, and customer satisfaction.

### 3. Introduction to Data collected and Number of itemsets in the data

The data required for the analysis and conduction of Association rules was collected by circulating the google forms among the residentsof Bangalore and Belgaum. The details
of the google form are as follows.


<img width="381" alt="image" src="https://github.com/dhanashreehampiholi/Recommendation-System-for-purchase-at-Zepto/assets/57892263/06aad821-6055-4dfb-a6f6-4d68fa6646a0">


<img width="383" alt="image" src="https://github.com/dhanashreehampiholi/Recommendation-System-for-purchase-at-Zepto/assets/57892263/62000f38-22bd-4be9-b734-aeae444aa261">


<img width="383" alt="image" src="https://github.com/dhanashreehampiholi/Recommendation-System-for-purchase-at-Zepto/assets/57892263/7cb88865-3b2e-4bb1-9d90-6516fa837e69">


<img width="387" alt="image" src="https://github.com/dhanashreehampiholi/Recommendation-System-for-purchase-at-Zepto/assets/57892263/717584ec-0e30-4741-969c-8e71f09cef56">


<img width="361" alt="image" src="https://github.com/dhanashreehampiholi/Recommendation-System-for-purchase-at-Zepto/assets/57892263/b23d6fec-d52c-4c61-9d36-bb19bb4e7f2a">


<img width="484" alt="image" src="https://github.com/dhanashreehampiholi/Recommendation-System-for-purchase-at-Zepto/assets/57892263/830fb107-422e-4a72-9483-9b2996a49ccb">


### 4. Introduction to Data Methodology 

#### a. Data Preprocessing Steps followed

Data preprocessing is a crucial step in data analysis and machine learning. It involves cleaning and transforming raw data into a format that is more suitable for
analysis. Here are the general steps followed in data preprocessing:

##### Data Cleaning:

Handling missing data: Remove or impute missing values using techniques like mean, median, or mode imputation.

##### Handling outliers:

Identify and deal with outliers, either by removing them or transforming them.

##### Data deduplication:

Remove duplicate entries if any.

##### Correcting data format: 

Ensure all data types are correct and consistent.

##### Handling irrelevant data: 
Remove irrelevant features that do not contribute to the analysis.

#### Data Transformation:

##### Normalization: 

Scale numerical features to a standard range, such as [0, 1] or [-1,1].

##### Standardization:

Transform data to have a mean of 0 and a standard deviation of 1. 

##### Encoding categorical variables:

Convert categorical variables into numerical representations (e.g., one-hot encoding).

##### Discretization: 

Convert continuous data into discrete categories.

##### Feature engineering: 

Create new features based on existing ones to improve model performance.

#### Data Reduction:

##### Feature selection: 

Select a subset of relevant features to reduce dimensionality.

##### Dimensionality reduction: 

Use techniques like Principal Component Analysis (PCA) or Singular Value Decomposition (SVD) to reduce the number of features while retaining important information.
#### Data Integration:

Combine data from multiple sources into a single dataset, ensuring compatibility and consistency.

#### Data Discretization:

Convert continuous data into discrete form for analysis.

#### Data Normalization:

Scale the data to a specific range to ensure that all features contribute equally to the analysis.

#### Data Sampling:

If the dataset is imbalanced, perform sampling techniques such as oversampling or undersampling to balance the classes.

#### Data Splitting:

Split the dataset into training, validation, and test sets for model training and evaluation.

#### Data Augmentation:

Generate additional training data from existing data to improve model performance, often used in image or text data. Each of these steps is essential for preparing the data for analysis and ensuring that
the machine learning model can learn effectively from the data.

#### b. Association Rules

Association rules are used in data mining to find interesting relationships between variables in large databases. They are typically used for market basket analysis,
where the goal is to find associations between products that are frequently purchased together. The most common metric used to evaluate association rules is support, confidence, and lift.

##### Support: 
The support of an itemset is the proportion of transactions in the database in which the itemset appears together. It is calculated as the number of
transactions containing the itemset divided by the total number of transactions.

<img width="325" alt="image" src="https://github.com/dhanashreehampiholi/Recommendation-System-for-purchase-at-Zepto/assets/57892263/d73170cd-f0e3-4c9e-9bf7-00ed138773df">


##### Confidence:
The confidence of a rule (A -> B) is the proportion of transactions that contain A which also contain B. It is calculated as the support of (A ∪ B)
divided by the support of A.

<img width="475" alt="image" src="https://github.com/dhanashreehampiholi/Recommendation-System-for-purchase-at-Zepto/assets/57892263/c4686582-e808-46e0-bec2-8f782207c1be">


##### Lift: 
The lift of a rule (A -> B) measures how much more likely item B is to be bought when item A is bought, compared to when item B is bought regardless of item A. It is calculated as the confidence of the rule divided by the support of B.

<img width="313" alt="image" src="https://github.com/dhanashreehampiholi/Recommendation-System-for-purchase-at-Zepto/assets/57892263/bc590788-a702-4bbc-8d7b-22e63092f90b">

Association rules are often used in retail for market basket analysis, where retailers want to understand the relationships between products that are frequently
purchased together. They can also be used in other domains such as healthcare, fraud detection, and recommendation systems.


#### c. Interpretation of Association Rule Output

##### Interpretation and Insights:
The generated association rules were interpreted to extract insights into consumer preferences and purchasing behavior. Interpreting association rule output is essential for understanding the relationships
between items in a dataset and deriving actionable insights. Here's how you can interpret association rule output effectively:

 Rule Metrics:
Begin by examining the support, confidence, and lift values associated with each rule. These metrics provide quantitative measures of the rule's
significance and strength.

 Support: 
Indicates how frequently the itemset occurs in the dataset.

 Confidence: 
Measures the probability of the consequent item given the antecedent item.

 Lift: 
Compares the observed support of the rule to what would be expected if the items were independent.

 Identify High-Lift Rules: 
Focus on rules with lift values greater than 1, as they indicate a positive association between the antecedent and consequent items. These rules suggest that the items tend to occur together more often than expected by
chance.

 Understand Confidence Levels: 
Consider the confidence level of each rule to gauge the strength of the association. Higher confidence values imply stronger relationships between items. Rules with low confidence may indicate weaker
associations or potential areas for further investigation.

 Explore Support Levels: 
Evaluate the support values to understand the frequency of occurrence of each itemset in the dataset. Higher support values indicate that the
itemset is more common among transactions, while lower support values may signify niche or less frequent patterns.

 Consider Rule Interpretability: 
Assess the interpretability of the association rules by examining the antecedent and consequent itemsets. Rules should be logical and
meaningful in the context of the dataset and domain. Ensure that the rules make intuitive sense and align with prior knowledge or expectations.

 Prune Rules:
Depending on the objectives of your analysis, you may need to filter or prune the association rules to focus on the most relevant or actionable insights.
This could involve setting thresholds for support, confidence, or lift values or applying additional criteria based on domain knowledge.

 Visualize Results: 
Use visualizations such as scatter plots, network diagrams, or heatmaps to visualize the association rules and their key metrics. Visual
representations can help identify patterns, trends, and clusters within the data more effectively.
 
 Contextualize Findings: 
Interpret the association rule output within the broader context of the business problem or research objectives. Consider how the discovered patterns and relationships can inform decision-making, strategy
development, or operational improvements.

### INTRODUCTION TO THE RESULTS OBTAINED AND INFERENCES DRAWN

#### 1. Data preprocessing results with codes

##### Codes used

install.packages('arules')

library(arules)

fp.df <- read.csv(file.choose()) #"Association excel.csv"

fp.df

# remove first column and convert to matrix

fp.mat <- as.matrix(fp.df[, -1]);fp.mat

# convert the binary incidence matrix into a transactions database

Data.tr <- as(fp.mat, "transactions")

inspect(Data.tr)

itemFrequencyPlot(Data.tr)

#Convert the transaction data into matrix data

Data.mat<-as(Data.tr,"matrix");Data.mat

#convert the matrix data into binary matrix

Data.bin<-apply(Data.mat,c(1,2),as.numeric);Data.bin


<img width="354" alt="image" src="https://github.com/dhanashreehampiholi/Recommendation-System-for-purchase-at-Zepto/assets/57892263/f90ec70f-e615-4f52-804f-babdec96515e">


<img width="391" alt="image" src="https://github.com/dhanashreehampiholi/Recommendation-System-for-purchase-at-Zepto/assets/57892263/69aca8f3-c7fc-421b-8834-db57c01c017c">


<img width="410" alt="image" src="https://github.com/dhanashreehampiholi/Recommendation-System-for-purchase-at-Zepto/assets/57892263/8eddb694-cd51-4820-81cf-2d6dbec90f5b">


### 1. Interpretation:

The provided output appears to be the result of association rules mining, showing the association rules, their support, confidence, coverage, lift, and
count. Here's how to interpret the data:

lhs (Left-hand side) and rhs (Right-hand side): 
These columns represent the items involved in the association rule. For example, the first rule indicates
that there is a relationship between an empty set (no specific item on the left- hand side) and "Masala_Dryfruits" on the right-hand side.

Support: 
This indicates the proportion of transactions in the dataset that contain both the left-hand side and the right-hand side of the rule. For
instance, the support of 0.4285714 for the first rule means that 42.86% of transactions contain "Masala_Dryfruits".

Confidence:
Confidence measures how often the rule has been found to be true. It represents the likelihood that the right-hand side will be purchased when the left-hand side is purchased. For instance, a confidence of
0.4285714 for the first rule means that in 42.86% of transactions where "Masala_Dryfruits" is present, the left-hand side is also present.

Coverage: 
This indicates the proportion of transactions that contain the left- hand side of the rule. It represents the popularity of the left-hand side items.
A coverage of 1 means that the left-hand side is present in all transactions. 

Lift:
Lift measures how much more often the items in the association rule occur together than if they were statistically independent. A lift value of 1
indicates independence, while values greater than 1 indicate a positive correlation. For instance, a lift of 1 for the first rule means that there is no
association between the presence of "Masala_Dryfruits" and the other items.

Count: 
This column represents the absolute count of transactions that contain both the left-hand side and the right-hand side of the rule.
Overall, these association rules provide insights into the relationships between different products in the dataset, helping Zepto's recommendation
system identify patterns and make relevant product suggestions to customers.

### 2. Rule Generation using apriori algorithm







