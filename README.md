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

#remove first column and convert to matrix

fp.mat <- as.matrix(fp.df[, -1]);fp.mat

#convert the binary incidence matrix into a transactions database

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

#### ONE FREQUENT ITEMSETS OBTAINED

<img width="456" alt="image" src="https://github.com/dhanashreehampiholi/Recommendation-System-for-purchase-at-Zepto/assets/57892263/2b994283-fd66-47c2-8467-683b9812bc21">

The results presented are association rules generated from the Association excel dataset, indicating the relationships between different sets of products. Each
rule consists of an antecedent (lhs - left-hand side) and a consequent (rhs - right-hand side), along with various metrics such as support, confidence,
coverage, lift, and count.

##### 1. {Masala_Dryfruits }
Support: 0.42 (42% of transactions contain Masala_Dryfruits)
Confidence: 0.42 (42% of transactions that contain {} also Masala_Dryfruits)
Interpretation: This rule suggests that 42% of transactions involve the purchase of Masala_Dryfruits. The confidence of 42% indicates that when no other product is purchased, there is a chance of 42% that Masala_Dryfruits will be bought. Since the lift is 1.0, there is no significant association between the absence of other products.

##### 2. {Atta_Rice_Dal}
Support: 0.42 (42% of transactions contain Atta_Rice_Dal)
Confidence: 0.42 (42% of transactions that contain {} also contain Atta_Rice_Dal)
Interpretation: This rule says that 42% of transactions involve the purchase of Atta_Rice_Dal. The confidence off 42% interprets that when no other
product is purchased, there is a chance of 42% that Atta_Rice_Dal will be purchased. Since the lift is 1.0, there is no significant association between the
absence of other products.

##### 3. {Tea_Coffee }
Support: 0.46 (46% of transactions contain Tea_Coffee)
Confidence: 0.46 (46% of transactions that contain {} also contain Tea_Coffee)
Interpretation: In this rule the support of 46% suggests that 46% of transactions involve the purchase of Tea_Coffee. Followed by confidence of
46% interprets that when no other product is purchased, there is a chance of 46% that Tea_Coffee will be bought. Since the lift is 1.0, there is no
significant association between the absence of other products.

##### 4. {Packaged_food }
Support: 0.48 (48% of transactions contain Packaged_food)
Confidence: 0.48 (48% of transactions that contain {} also contain Packaged_food)
Interpretation: This rule says that 48% of transactions involve the purchase of Packaged_food. The confidence off 48% interprets that when no other
product is purchased, there is a chance of 48% that Packaged_food will be purchased. Since the lift is 1.0, there is no significant association between the
absence of other products.

##### 5. {Sweets }
Support: 0.51 (51% of transactions contain Sweets)
Confidence: 0.51 (51% of transactions that contain {} also contain Sweets)
Interpretation: : In this rule the support of 51% suggests that 51% of transactions involve the purchase of Sweets. Followed by confidence of 51% interprets that when no other product is purchased, there is a chance of 51% that Sweets will be bought. Since the lift is 1.0, there is no significant association between the absence of other products.

##### 6. {Dairy_bread}
Support: 0.55 (55% of transactions contain Dairy_bread)
Confidence: 0.55 (55% of transactions that contain {} also contain Dairy_bread)
Interpretation: : In this rule the support of 55% suggests that 55% of transactions involve the purchase of Dairy_bread. Followed by confidence of 55% interprets that when no other product is purchased, there is a chance of 55% that Dairy_bread will be bought. Since the lift is 1.0, there is no significant association between the absence of other products.

##### 7. {ColdDrinks_Juice}
Support: 0.55 (55% of transactions contain ColdDrinks_Juice)
Confidence: 0.55 (55% of transactions that contain {} also contain ColdDrinks_Juice)
Interpretation: : In this rule the support of 55% suggests that 55% of transactions involve the purchase of ColdDrinks_Juice. Followed by confidence of 55% interprets that when no other product is purchased, there is a chance of 55% that ColdDrinks_Juice will be bought. Since the lift is 1.0, there is no significant association between the absence of other products.

##### 8. {Biscuits_Cookies}
Support: 0.57 (57% of transactions contain Biscuits_Cookies)
Confidence: 0.57 (57% of transactions that contain {} also contain Biscuits_Cookies)
Interpretation: : In this rule the support of 57% suggests that 57% of transactions involve the purchase of Biscuits_Cookies. Followed by confidence of 57% interprets that when no other product is purchased, there is a chance of 57% that Biscuits_Cookies will be bought. Since the lift is 1.0, there is no significant association between the absence of other products.

##### 9. {Breakfast_Sauces}
Support: 0.59 (59% of transactions contain Breakfast_Sauces)
Confidence: 0.59 (59% of transactions that contain {} also contain Breakfast_Sauces)
Interpretation: : In this rule the support of 59% suggests that 59% of transactions involve the purchase of Breakfast_Sauces. Followed by
confidence of 59% interprets that when no other product is purchased, there is a chance of 59% that Breakfast_Sauces will be bought. Since the lift is 1.0,
there is no significant association between the absence of other products.

##### 10.{FrozenFood and Icecream}
Support: 0.61 (61% of transactions contain FrozenFood and Icecream)
Confidence: 0.61 (61% of transactions that contain {} also contain FrozenFood and Icecream)
Interpretation: : In this rule the support of 61% suggests that 61% of transactions involve the purchase of FrozenFood and Icecream. Followed
by confidence of 61% interprets that when no other product is purchased, there is a chance of 61% that FrozenFood and Icecream will be bought. Since the lift is 1.0, there is no significant association between the absence of other products.

##### 11.{Munchies_Chips}
Support: 0.61 (61% of transactions contain Munchies_Chips)
Confidence: 0.61 (61% of transactions that contain {} also contain Munchies_Chips)
Interpretation: : In this rule the support of 61% suggests that 61% of transactions involve the purchase of Munchies_Chips. Followed by confidence of 61% interprets that when no other product is purchased, there is a chance of 61% that Munchies_Chips will be bought. Since the lift is 1.0, there is no significant association between the absence of other products.

##### 12.{Others}
Support: 0.53 (53% of transactions contain Munchies_Chips)
Confidence: 0.53 (53% of transactions that contain {} also contain Munchies_Chips)
Interpretation: : In this rule the support of 53% suggests that 53% of transactions involve the purchase of Munchies_Chips. Followed by confidence of 53% interprets that when no other product is purchased, there is a chance of 53% that Munchies_Chips will be bought. Since the lift is 1.0, there is no significant association between the absence of other products.

These rules suggest strong associations between the empty set and each individual product category, indicating that these products are commonly purchased alone.

<img width="409" alt="image" src="https://github.com/dhanashreehampiholi/Recommendation-System-for-purchase-at-Zepto/assets/57892263/9a04ee66-adc5-49c5-ac15-6575e4069684">

<img width="404" alt="image" src="https://github.com/dhanashreehampiholi/Recommendation-System-for-purchase-at-Zepto/assets/57892263/81eb8ca5-432c-4eab-a6c1-4d8b97906d09">

This is a pair plot which again gives a visual representation using parameters like support, Confidence, Coverage, Lift and Count.

<img width="399" alt="image" src="https://github.com/dhanashreehampiholi/Recommendation-System-for-purchase-at-Zepto/assets/57892263/617e21bc-5065-4e1b-bc36-41fe250da8fc">

Interpretation: the scatter plot, gives a visual representation of the generated rules plotted by support against the confidence . By considering the cutoff level of 0.02 for support and 0.01 for confidence and a lift of 1 we filter only few rules of 1 frequent itemsets to take into consideration.

<img width="370" alt="image" src="https://github.com/dhanashreehampiholi/Recommendation-System-for-purchase-at-Zepto/assets/57892263/d6801866-c42b-4883-a0fe-461059b2745c">

#### TWO FREQUENT ITEMSETS OBTAINED

<img width="440" alt="image" src="https://github.com/dhanashreehampiholi/Recommendation-System-for-purchase-at-Zepto/assets/57892263/179b03ba-31ec-452e-8b4a-10e1ecc90002">

#### INTERPRETATION
The association rules mined from the dataset reveal interesting patterns in customer purchasing behavior within Zepto's product categories:
 Customers who purchase Packaged Food are likely to also purchase Frozen Food and Ice Cream. This association has a high confidence of 0.75, indicating strong support
for the rule.
 Cold Drinks and Juice buyers are highly inclined to purchase Munchies Chips as well, with a confidence of 0.7777 and support of 0.4285.
 Munchies Chips purchasers often accompany their purchase with Cold Drinks and Juice, with a similar confidence of 0.7.
 Customers who buy items categorized as Others are often interested in Biscuits and Cookies, with a confidence of 0.6923.
 Biscuits and Cookies buyers also tend to purchase Others, supporting the notion that these items are commonly bought together, with a confidence of 0.6429.
There is a significant association between Others and Breakfast Sauces, indicating a potential cross-category buying behavior, with a confidence of 0.7692.
 The reciprocal relationship holds, with Breakfast Sauces buyers likely to purchase Others as well, albeit with slightly lower confidence.
 Biscuits and Cookies purchasers show an inclination towards Frozen Food and Ice Cream as well as Munchies Chips, with confidence levels of 0.6429 each.
 Breakfast Sauces buyers exhibit a preference for Frozen Food and Ice Cream, suggesting a trend of purchasing condiments alongside frozen treats.

Thus, looking at all the 4 parameters, we can conclude that, rule 2,3,6, and 7 are appropriate for implementation purpose. Thus, the shop owner can give discount
for customers purchasing the above combinations i.e ColdDrinks_Juice, Munchies_Chips, Breakfast_Sauces and Others.

<img width="323" alt="image" src="https://github.com/dhanashreehampiholi/Recommendation-System-for-purchase-at-Zepto/assets/57892263/c3bf2fca-5913-4390-98d4-fa47587dcb7b">

From the above scatter plot we can see that all the rules have a support below 42%, where confidence is 77% and below.

<img width="288" alt="image" src="https://github.com/dhanashreehampiholi/Recommendation-System-for-purchase-at-Zepto/assets/57892263/9982d90d-f351-402a-a516-8a6e2845d9ef">

<img width="286" alt="image" src="https://github.com/dhanashreehampiholi/Recommendation-System-for-purchase-at-Zepto/assets/57892263/3f8ceeda-06ea-4970-920a-f6dbbbc4729e">

#### THREE FREQUENT ITEMSETS

<img width="458" alt="image" src="https://github.com/dhanashreehampiholi/Recommendation-System-for-purchase-at-Zepto/assets/57892263/d0eb406c-3c4f-44e2-ad2d-a655ce23d137">

##### INTERPRETATION
The association rules extracted from the dataset provide deeper insights into the relationships between multiple items and their impact on customer purchasing behavior within Zepto's product categories:

 Customers who purchase Packaged Food and Others together are highly likely to also purchase Frozen Food and Ice Cream. This association rule has a high
confidence of 0.8462, indicating strong support for the rule.
 Customers who buy Packaged Food alongside Breakfast Sauces have a high probability of purchasing Frozen Food and Ice Cream as well, with a confidence
of 0.9231.
 For customers purchasing Sweets and Cold Drinks or Juice together, there's a strong likelihood of also buying Munchies Chips, supported by a confidence of
0.8462.
 Customers who purchase Sweets and Others together are inclined to add Breakfast Sauces to their cart as well, with a confidence of 0.8571.
 The association between Cold Drinks or Juice and Others also extends to Munchies Chips, with a confidence of 0.8462, indicating a consistent buying
pattern across these items.
 Customers purchasing Cold Drinks or Juice alongside Breakfast Sauces are highly likely to also purchase Munchies Chips, with a confidence of 0.8750.

These association rules highlight the interplay between different product categories and can inform Zepto's marketing strategies, product bundling, and recommendation system to enhance customer engagement and satisfaction while driving sales.

Thus, looking at all the 4 parameters, we can conclude that, rule 2,3 are appropriate for implementation purpose. Thus, the shop owner can give discount for customers purchasing the above combinations of screen protector and phone insurance and Memory card.

<img width="412" alt="image" src="https://github.com/dhanashreehampiholi/Recommendation-System-for-purchase-at-Zepto/assets/57892263/d78f83a0-fd85-4d77-b905-1a1016cf55f2">

In the above scatter plot we can see that the support for all the rules is very less which is 28% and below where as confidence is high which is 93% and below.

<img width="367" alt="image" src="https://github.com/dhanashreehampiholi/Recommendation-System-for-purchase-at-Zepto/assets/57892263/2db24df7-d4b3-47d5-bf76-4c67f4f00270">

<img width="375" alt="image" src="https://github.com/dhanashreehampiholi/Recommendation-System-for-purchase-at-Zepto/assets/57892263/404ef00f-1229-4aef-aedb-b3fa5648bc13">

#### 4-FREQUENT ITEMSETS OBTAINED

<img width="468" alt="image" src="https://github.com/dhanashreehampiholi/Recommendation-System-for-purchase-at-Zepto/assets/57892263/fb52200a-9765-4653-b9bc-def3ed92f6b6">

The association rules mined from the dataset continue to reveal interesting patterns in customer purchasing behavior within Zepto's product categories, with some
combinations showing strong associations:

Transactions where customers purchase Packaged Food, Dairy Bread, and Breakfast Sauces together are highly likely to also include Frozen Food and
Ice Cream, with a confidence of 1.0. This indicates a consistent buying pattern among these items.

 Similarly, customers who buy Packaged Food, Biscuits and Cookies, and Others together are inclined to also purchase Frozen Food and Ice Cream, with a high confidence of 0.9.

 Transactions involving Packaged Food, Breakfast Sauces, and Others also show a strong association with Frozen Food and Ice Cream, supported by a confidence of 1.0.

 For customers purchasing Sweets, Cold Drinks or Juice, and Breakfast Sauces together, there's a high likelihood of also purchasing Munchies Chips, with a confidence of 1.0.

 Additionally, transactions where Cold Drinks or Juice, Breakfast Sauces, and Others are bought together also exhibit an association with Munchies
Chips, albeit with a slightly lower confidence of 0.9.

Thus, looking at all the 4 parameters, we can conclude that, rule 3 is the most appropriate for implementation purpose. Thus, the shop owner can give discount
for customers purchasing the above combination of Packaged_food, Breakfast_Sauces and Others.

<img width="406" alt="image" src="https://github.com/dhanashreehampiholi/Recommendation-System-for-purchase-at-Zepto/assets/57892263/b0a6273a-18d3-48ef-be8d-7a2fcca27194">

<img width="357" alt="image" src="https://github.com/dhanashreehampiholi/Recommendation-System-for-purchase-at-Zepto/assets/57892263/c5441ca2-a09c-4d1b-8841-d762b758fc12">

### 3. Assessing the strength of the rules obtained

To assess the strengths of the rules obtained, we can consider several aspects:
Support: The support value indicates how frequently a rule occurs in the dataset. Higher support values suggest that the rule is applicable to a larger portion of transactions.
Confidence: Confidence measures the reliability of the rule. A high confidence value indicates that the consequent (rhs) is likely to be true when the antecedent
(lhs) is true.
Lift: Lift compares the likelihood of the consequent under the conditions of the rule to the likelihood of the consequent without regard to the antecedent. A lift
value greater than 1 indicates that the rule has a positive effect on the likelihood of the consequent.
Coverage: Coverage measures the proportion of instances in the dataset that are covered by the rule. Higher coverage values indicate that the rule applies to a larger portion of the dataset.

## IV. CONCLUSION
#### Recommendation from the analysis
From the above analysis we can interpret that there are several combinations of products where the Zepto store can provide discounts and offers .The combinations
include

 1-frequent itemset
Munchies_Chips
FrozenFood_Icecreams

 2-frequent itemset
PackagedFood and Icecream
Munchies_Chips and Cold drinks


 3-frequent itemsets
PackagedFood, Breakfast_Sauces and Frozenfood_Icecreams

 4-frequent itemsets
 PackagedFood, Breakfast_Sauces , Frozenfood_Icecreams and Dairy bread


 ## V. CODE USED
##################################################
#Purchases of Items on Zepto
install.packages('arules')
library(arules)
fp.df <- read.csv(file.choose()) #"Association excel.csv"
fp.df
#remove first column and convert to matrix
fp.mat <- as.matrix(fp.df[, -1]);fp.mat
#convert the binary incidence matrix into a transactions database
Data.tr <- as(fp.mat, "transactions")
inspect(Data.tr)
itemFrequencyPlot(Data.tr)

#Convert the transaction data into matrix data
Data.mat<-as(Data.tr,"matrix");Data.mat
#convert the matrix data into binary matrix
Data.bin<-apply(Data.mat,c(1,2),as.numeric);Data.bin
##get rules
#when running apriori(), include the minimum support, minimum confidence,
#and target as arguments.
##########################################
##requent 1-itemsets
Data.freq1 <- apriori(Data.bin, parameter=list(minlen=1, maxlen=1, support=0.02,

target="frequent itemsets"))
summary(Data.freq1)
inspect(head(sort(Data.freq1, by = "support"), 10))
rules <- apriori(Data.bin, parameter=list(minlen=1,maxlen=1,support=0.02,
confidence=0.01, target = "rules"))
summary(rules)
inspect(rules)
install.packages('arulesViz')
library(arulesViz)
plot(rules)
#Notice that rules are clustered at two places.
#If support >=0.2 and confidence >=0.7 and lift >=1, we will
#consider rules
#Thus, only those clusters at top right corner are considered
plot(rules@quality)
inspect(head(sort(rules, by = "support"), n = 20))
highsupportRules <- head(sort(rules, by="support"), 10)
plot(highsupportRules, method="graph", control=list(type="items"))
highLiftRules <- head(sort(rules, by="lift"), 20)
plot(highLiftRules,control=list(type="items"))

##frequent 2-itemsets (we will keep support=0.2)-Notice same results in excel
Data.freq2 <- apriori(Data.bin, parameter=list(minlen=2, maxlen=2, support=0.02,
target="frequent itemsets"))
summary(Data.freq2)
inspect(head(sort(Data.freq2, by = "support"), 10))

###################################
##frequent 2-itemsets (Rule Generation and Visualization)
#(we will keep support=0.2 and confidence =0.7)-Notice same results in excel
rules <- apriori(Data.bin, parameter=list(minlen=2,maxlen=2,support=0.35,
confidence=0.642, target = "rules"))
summary(rules)
inspect(rules)
install.packages('arulesViz')
library(arulesViz)
plot(rules)
#Notice that rules are clustered at two places.
#If support >=0.2 and confidence >=0.7 and lift >=1, we will
#consider rules
#Thus, only those clusters at top right corner are considered
plot(rules@quality)
inspect(head(sort(rules, by = "support"), n = 20))
highsupportRules <- head(sort(rules, by="support"), 10)
plot(highsupportRules, method="graph", control=list(type="items"))
highLiftRules <- head(sort(rules, by="lift"), 20)
plot(highLiftRules,method="graph",control=list(type="items"))

###################################
#frequent 3-itemsets
Data.freq3<- apriori(Data.bin, parameter=list(minlen=3, maxlen=3, support=0.02,
target="frequent itemsets"))
inspect(sort(Data.freq3, by ="support"))
##frequent 3-itemsets (Rule Generation and Visualization)
#(we will keep support=0.2 and confidence =0.7)
rules <- apriori(Data.bin, parameter=list(minlen=3,maxlen=3,support=0.2,
confidence=0.84, target = "rules"))
summary(rules)
inspect(rules)
library(arulesViz)
plot(rules,main="scatterplot of 6 rules")
plot(rules,main="scatterplot of 6 rules",jitter=0)
#Notice that rules are clustered at two places.
#If support >=0.2 and confidence >=0.7 and lift >=1, we will
#consider rules
#Thus, only those clusters at top left corner are considered
plot(rules@quality)
inspect(head(sort(rules, by = "support"), n = 20))
highsupportRules <- head(sort(rules, by="support"), 10)
plot(highsupportRules, method="graph", control=list(type="items"))
highLiftRules <- head(sort(rules, by="lift"), 20)
plot(highLiftRules,method="graph",control=list(type="items"))

####################################
#frequent 4-itemsets (no items exist)
Data.freq4 <- apriori(Data.bin, parameter=list(minlen=4, maxlen=4, support=0.02,
target="frequent itemsets"))
inspect(sort(Data.bin, by ="support"))
inspect(head(sort(rules, by = "support"), n = 20))
rules <- apriori(Data.bin, parameter=list(minlen=4,maxlen=4,support=0.15,
confidence=0.9, target = "rules"))
summary(rules)
inspect(rules)
plot(rules,main="scatterplot of 5 rules")
plot(rules,main="scatterplot of 5 rules",jitter=0)
plot(rules@quality)
highsupportRules <- head(sort(rules, by="support"), 10)
plot(highsupportRules, method="graph", control=list(type="items"))
highLiftRules <- head(sort(rules, by="lift"), 20)
plot(highLiftRules,method="graph",control=list(type="items"))

################
#if we do not specify the minlen and maxlen, we get all the rules

rules <- apriori(Data.bin, parameter = list(supp = 0.2, conf = 0.7,
target = "rules"))
#inspect the first ten rules, sorted by their support
inspect(head(sort(rules, by = "support"), n = 10))
highsupportRules <- head(sort(rules, by="support"), 6)
plot(highsupportRules, method="graph", control=list(type="items"))
highLiftRules <- head(sort(rules, by="lift"), 5)
plot(highLiftRules, method="graph", control=list(type="items"))
#select the 5 rules with the highest support
highsupportRules <- head(sort(rules, by="support"), 6)
plot(highsupportRules, method="graph", control=list(type="items"))
#Notice that, size of circles is based on support size. Since the rule
#{ }--> "white" is 0.7 we have bigger circle size.
#Notice the color of circle is based on lift strength.
#greater the lift -->darker the color
#The arrows point towards the rules seen in the output.
#select the 5 rules with the highest lift
highLiftRules <- head(sort(rules, by="lift"), 5)
plot(highLiftRules, method="graph", control=list(type="items"))




















