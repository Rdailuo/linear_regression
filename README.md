# Linear Regression Project

For this project, imagine the context: we just got some contract work with an Ecommerce company based in New York City that sells clothing online but they also have in-store style and clothing advice sessions. Customers come in to the store, have sessions/meetings with a personal stylist, then they can go home and order either on a mobile app or website for the clothes they want.

The company is trying to decide whether to focus their efforts on their mobile app experience or their website. They've hired us on contract to help them figure it out! Let's get started!

Click here to view the notebook: [Linear Regression.ipynb]

## About the Data: 

The dataset includes customer information and engagement metrics:

**Email**: Customer email (identifier) \
**Address**: Customer location (identifier) \
**Avatar**: Profile image (identifier)\
**Avg. Session Length**: Average session duration in minutes\
**Time on App**: Minutes spent on the mobile app\
**Time on Website**: Minutes spent on the website\
**Length of Membership**: Membership duration in years\
**Yearly Amount Spent**: Target variable representing total yearly spending

## Key Technical Tools:

**Python Libraries**: pandas for data handling, numpy for numerical operations, and seaborn & matplotlib for visualizations\
**Scikit-Learn**: Used for regression modeling and model training

## Key Plots Used: 
**Pairplots**: Used pair plot to explore these types of relationships across the entire data set. Observed that Length of Membership is most correlated with Yearly Amount Spent\
**Scatterplot**: After predicting the testing data, we created a scatterplot of the real test values versus the predicted values \
**Residual Plot**: Examines residuals to assess model accuracy, confirming the appropriateness of a linear regression model\

## After running regression, we interpreted the coefficients: 
<img width="325" alt="Screenshot 2024-11-03 at 12 53 45 PM" src="https://github.com/user-attachments/assets/8ed58811-e862-44fb-b49b-804b894659a4">

**Let's interpret those coefficients**

Holding all other features fixed, a 1 unit increase in Avg. Session Length is associated with an increase of 25.98 total dollars spent.\
Holding all other features fixed, a 1 unit increase in Time on App is associated with an increase of 38.59 total dollars spent.\
Holding all other features fixed, a 1 unit increase in Time on Website is associated with an increase of 0.19 total dollars spent.\
Holding all other features fixed, a 1 unit increase in Length of Membership is associated with an increase of 61.27 total dollars spent.

**Should this company focus on their mobile app or on their website?**

Based on the regression results, it appears that Time on App drives spending far more effectively than Time on Website — with each unit of app time linked to an additional $38.59 spent, compared to just $0.19 for the website. This suggests that enhancing the mobile app would yield immediate revenue benefits, as it’s already the stronger channel.\

However, this is tricky and there are two ways to think about this: Develop the Website to catch up to the performance of the mobile app, or develop the app more since that is what is working better. This sort of answer really depends on the other factors going on at the company, we can further explore the relationship between Length of Membership and the App or the Website before coming to a conclusion!

Visualize the results and plots in the Notebook. 

