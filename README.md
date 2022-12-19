# Product-Oriented Social Media Sentiment Analysis Webapp
The purpose of this web application is to perform sentiment analysis of social media data to determine the overall sentiment of customers towards a company's product or service, and identify common themes or issues in customer feedback. This project aims to provide companies with a valuable tool for understanding and improving the perception of their products or services among their customers

# Abstract



# Introduction
The subject of this proposal is a potential development of a web application for performing sentiment analysis of social media data to determine the overall sentiment of customers towards a company's product or service, and identify common themes or issues in customer feedback. This project aims to provide companies with a valuable tool for understanding and improving the perception of their products or services among their customers.

The report is structured as follows: The literature review section provides an overview of the existing research and approaches to sentiment analysis, as well as the relevant technology and tools used in the proposed web application. The problem statement section outlines the motivation and rationale for the project, including the gap in the current market and the potential benefits of the proposed web application. The methodology section outlines the approach and steps taken to develop the web application, including the data collection and pre-processing, storage, analysis, and visualization components. The system design and analysis section contains the interface design, functional and non-functional requirements, and overall system architecture of the proposed web application.

In acknowledging the existing work in the field of sentiment analysis, this project builds upon and extends previous research by incorporating the latest technology and tools, and applying them to the specific context of social media data from multiple platforms (Twitter, Facebook, and Instagram). The scope of this project is limited to the development and evaluation of the proposed web application, and does not include any broader market analysis or business strategy recommendations. The project schedule for the development of the web application is outlined in the methodology section.

Overall, this report aims to provide a comprehensive overview of the proposed web application for sentiment analysis of social media data, and to demonstrate its potential value and feasibility as a tool for companies to understand and improve the perception of their products or services among their customers.

# Objectives

1. Determine the overall sentiment of customers towards the company's product or service: This objective involves analyzing the language used by customers in their social media posts and determining whether the sentiment is positive, negative, or neutral. This can be measured by calculating the percentage of positive, negative, and neutral posts, as well as by tracking changes in sentiment over time.

2. Identify common themes or issues in customer feedback: By analyzing the content of social media posts, the webapp can identify common themes or issues that are frequently mentioned by customers. This can help the company identify areas where it may need to improve its product or service.

3. Monitor for potential crises or negative events: By tracking social media sentiment in real-time, the webapp can alert the company to any potential crises or negative events that may be developing. This can help the company respond quickly and effectively to these situations.

4. Provide insights for marketing and customer service: The data collected through social media sentiment analysis can be used to inform marketing and customer service strategies, helping the company understand what customers like and dislike about its product or service, and how it can better meet their needs.

5. Increase customer satisfaction: By using the insights gained through social media sentiment analysis, the company can take steps to improve its product or service, leading to increased customer satisfaction. This can be measured through customer satisfaction surveys or other metrics.

# Literature Review


# Problem Statements
1. The company has a clear understanding of how customers feel about its product or service, and can use this information to make informed decisions about how to improve and market its offerings. **The company lacks a reliable way to track and analyze customer sentiment on social media. As a result, it is unable to accurately gauge how customers feel about its product or service, and may be missing out on valuable insights**. Creating a social media sentiment analysis webapp that allows the company to track and analyze customer sentiment on social media in real-time. This will enable the company to identify trends and patterns in customer feedback, identify common themes or issues, and respond quickly to potential crises or negative events.

2. The company is able to identify and address customer complaints and issues in a timely manner, leading to increased customer satisfaction. **The company is unaware of many customer complaints or issues because they are not being shared on social media or are being shared in a way that is difficult to track. As a result, the company is unable to address these issues and may be losing customers as a result**. Creating a social media sentiment analysis webapp that allows the company to monitor social media for customer complaints and issues. This will enable the company to identify and address these issues in a timely manner, leading to increased customer satisfaction.

# Methodology
1. Define the project objectives: The first step will be to clearly define the objectives of the project. This will involve identifying the specific questions that the webapp is intended to answer, such as the overall sentiment of customers towards the company's product or service, common themes or issues in customer feedback, and the potential for negative events or crises.

2. Identify the target audience: Next, it will be important to identify the specific social media platforms and user groups that the webapp will target. This will involve researching the demographics and online behavior of the target audience, as well as determining which platforms they are most active on.

3. Collect and organize the data: The webapp will then need to collect and organize data from the targeted social media platforms. This will involve using appropriate data-gathering techniques, such as web scraping or API access, to gather relevant posts and comments from the targeted platforms. The data will then need to be cleaned and organized in a way that allows for easy analysis.

4. Store the data: The webapp will be able to store said data into a long term database storage, preferably on a secure and trusted 3rd party service provider for future queries and history tracking.

5. Analyze the data: Once the data has been collected and organized, it can be analyzed using appropriate tools and techniques. This may involve using natural language processing to identify the sentiment of individual posts, or using statistical analysis to identify trends and patterns in the data.

6. Present the results: The final step will be to present the results of the analysis in a clear and concise manner. This may involve creating visualizations, such as charts and graphs, to illustrate the findings, as well as writing a report that summarizes the key takeaways.

Throughout this process, it will be important to ensure that the data-gathering techniques used are appropriate and ethical, and that the results of the analysis are presented in a way that is accurate and unbiased.

# System Analysis and Design
The proposed web application is designed to collect and stream data from popular social media platforms such as Twitter, Facebook, and Instagram via their respective APIs. The data collected from these platforms will be pre-processed and loaded into a MySQL database for storage and analysis. The web application will then use sentiment analysis algorithms to analyze the data and generate data visualizations that will be displayed on an interactive front-end web app. The web app will be written in R and deployed as a Shiny web app to provide users with a seamless and intuitive interface for interacting with the data and visualizations.

## Interface Design
The interface design for the proposed web application will be clean and user-friendly, with a focus on simplicity and ease of use. The main dashboard will display the data visualizations generated by the sentiment analysis algorithms, along with a search bar that allows users to search for specific terms or hashtags within the data. There will also be a menu bar at the top of the page that allows users to navigate to different sections of the app, such as the data visualization page, the data management page, and the settings page.

The data visualization page will display a range of interactive graphs and charts that allow users to explore the data in greater detail. These visualizations will include bar charts, line graphs, and pie charts, and will be generated using popular visualization libraries such as ggplot2 and plotly. Users will be able to interact with the visualizations by hovering over individual data points, zooming in and out, and filtering the data by specific criteria.

The data management page will allow users to view, edit, and delete the data that has been collected and stored in the MySQL database. This page will also allow users to import new data from the social media APIs and add it to the database.

The settings page will allow users to configure the app's settings, such as the data sources to be collected from and the frequency of data collection. Users will also be able to change their password and logout from the app on this page.

## System Design
The proposed web application will be built using a combination of R, Shiny, and MySQL. R will be used as the primary programming language for the app, with Shiny providing the framework for building interactive web applications. MySQL will be used as the database management system for storing and analyzing the collected data.

The web application will collect data from the social media APIs using the rtweet, Rfacebook, and Rinstagram packages. These packages allow users to authenticate their accounts with the APIs and retrieve data in real-time or on a scheduled basis. The data collected from the APIs will be pre-processed using R's data manipulation and cleaning functions, and then loaded into the MySQL database using the RMySQL package.

Once the data has been stored in the MySQL database, the web application will use sentiment analysis algorithms to analyze the data and generate data visualizations. These visualizations will be generated using popular R visualization libraries such as ggplot2 and plotly, and will be displayed on the front-end web app using Shiny's interactive plotting functions.

## Functional Requirements
The functional requirements for the proposed web application are as follows:

1. The web application should be able to authenticate users with their social media accounts and retrieve data from the APIs in real-time or on a scheduled basis.
2. The web application should be able to pre-process the data collected from the APIs and store it in a MySQL database.
3. The web application should be able to analyze the data using sentiment analysis algorithms and generate data visualizations.
4. The web application should be able to display the data visualizations on an interactive front-end web app using Shiny.

## Non-Functional Requirements
The non-functional requirements for the proposed web application are as follows:

1. The web application should have a user-friendly interface that is visually appealing.
2. The web application should have good performance and be able to handle a large volume of data efficiently.
3. The web application should be secure and protect the collected data from unauthorized access.
4. The web application should be scalable and able to handle an increase in the volume of data collected or the number of users accessing the application.

# Conclusion


# References
https://github.com/ropensci/rtweet
https://github.com/trinker/sentimentr
https://cran.r-project.org/web/packages/SentimentAnalysis
https://benwiseman.github.io/sentiment.ai
https://dgarcia-eu.github.io/SocialDataScience/3_Affect/035_UnsupervisedToolsR/UnsupervisedToolsR.html
https://shiny.rstudio.com/





