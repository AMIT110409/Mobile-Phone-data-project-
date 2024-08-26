Mobile Phone Data Project
Project Overview
This project involves performing exploratory data analysis (EDA) on a dataset of mobile phones. The analysis includes univariate and bivariate analysis to understand the distribution and relationships between different features. Additionally, we predict phone ratings based on other features and cluster phones into groups based on their specifications.

Dataset
The dataset contains information about mobile phones, including features such as:

Battery: Battery capacity and details
Camera: Rear and front camera specifications
Display: Display size and type
Memory: RAM and internal storage capacity
Name: Name of the phone model
Price: Price of the phone
Processor: Processor details
Rating: User rating of the phone
Reviews: Number of user reviews
Warranty: Warranty information
The dataset has some missing values in the processor, rating, reviews, and warranty columns.

Objectives
Exploratory Data Analysis (EDA):

Univariate Analysis: Analyze the distribution of individual columns such as price and rating.
Bivariate Analysis: Investigate relationships between key features, particularly focusing on price and rating.
Bonus Tasks:

Rating Prediction: Develop a model to predict phone ratings based on other features.
Clustering: Group phones into clusters based on their specifications.
Installation and Requirements
Clone the repository:

bash
Copy code
git clone https://github.com/yourusername/mobile-phone-data-project.git
Install the required packages: Make sure you have Python 3.x installed. Then, run the following command to install dependencies:

bash
Copy code
pip install -r requirements.txt
Here are some key libraries used:

pandas: For data manipulation and cleaning.
seaborn and matplotlib: For data visualization.
scikit-learn: For predictive modeling and clustering.
Data Preprocessing
Before performing any analysis, missing values were handled:

Rating: Missing values were replaced with the median rating.
Processor: Missing values were replaced with the mode (most frequent processor).
Reviews and Warranty: Missing values were filled with placeholders such as "No Reviews" or "No Warranty Info."
Analysis
1. Univariate Analysis
We analyzed individual features to understand their distribution. For instance:

The price column showed a right-skewed distribution, indicating more phones are in the lower price range.
The rating column was left-skewed, with most ratings above 4.0.
2. Bivariate Analysis
We explored relationships between two variables, such as price and rating. A moderate positive correlation was found between them, indicating that higher-priced phones tend to have better ratings.

Bonus Tasks
1. Rating Prediction
A machine learning model (Random Forest Regressor) was used to predict phone ratings based on features like price, processor, camera, and memory. The model achieved a reasonable performance, as measured by metrics like R-squared and Mean Squared Error (MSE).

2. Clustering
We applied KMeans clustering to group phones based on their specifications. After reducing dimensionality using PCA, we visualized the clusters and found distinct groups of phones based on their attributes.

Running the Code
Exploratory Data Analysis: Run the script to generate visualizations and summary statistics:

bash
Copy code
python eda.py
Modeling: Train the model to predict phone ratings and evaluate performance:

bash
Copy code
python model.py
Clustering: Run the clustering analysis and visualize the results:

bash
Copy code
python clustering.py
Results and Insights
Price and Rating: Higher-priced phones generally receive better ratings, although there is some variation.
Phone Clusters: Phones were grouped into distinct clusters based on features such as battery life, camera specs, and price, offering insights into different segments in the mobile market.
Future Improvements
Feature Engineering: Enhance the model by engineering new features from the existing ones (e.g., combining camera specs or battery life into a single feature).
Advanced Modeling: Experiment with different machine learning models (e.g., Gradient Boosting or XGBoost) for better rating prediction.
Additional Clustering Techniques: Explore hierarchical clustering or DBSCAN for alternative clustering approaches.
Contributors
Amit Rathore 
License
This project is licensed under the MIT License - see the LICENSE file for details.

