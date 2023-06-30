# Project Name: A Serverless App For Spotify Data Processing Using AWS

Project Summary:
The goal of this project is to create a reliable and efficient data pipeline that extracts data from the Spotify API, transforms it, and loads it into a normalized DynamoDB database. The data can be accessed through an API Gateway and visualized on the front-end using HTML, CSS, and Chart.js. The project showcases the utilization of various AWS services to develop a secure, scalable, and efficient data pipeline for retrieving, transforming, and visualizing external data.

![image](https://github.com/Ali1999-AK/A-Serverless-App-Spotify/assets/63508161/ed8d7c3f-eced-4d9b-a8e8-aa71321d9a97)
![image](https://github.com/Ali1999-AK/A-Serverless-App-Spotify/assets/63508161/04df6bfa-36bf-4ff1-beb3-72918274d199)


Section 1:
Web Application URL:
The deployed web application can be accessed at http://100.24.36.101:3000/

GitHub Repository:
The source code for this project can be found on GitHub: https://github.iu.edu/vsaketh/team_mission_possible

Section 2:
Project Objectives and Usefulness:
The main objectives of this project are:

Develop a reliable, secure, and scalable data pipeline for extracting, transforming, and loading data from the Spotify API into DynamoDB.
Provide users with an interactive interface to access and analyze Spotify data, enabling them to gain insights into music preferences and behaviors.
Showcase the utilization of AWS services to build a robust and efficient data pipeline that can be adapted to different industries and use cases.
The project's usefulness includes:

Enabling music enthusiasts, marketers, and researchers to access and analyze Spotify data, leading to a better understanding of music trends, patterns, and behaviors.
Offering an interactive interface for users to visualize and analyze data in different formats, such as line charts, bar charts, and pie charts, facilitating comprehensive data exploration.
Demonstrating the power and flexibility of AWS services, providing a blueprint for developers and organizations to build scalable and reliable data pipelines for their own use cases.
Compared to other databases, this project stands out in the following ways:

Utilizes real-time data from the Spotify API, ensuring up-to-date and accurate information on music preferences and behaviors.
Built on AWS services, providing scalability, reliability, and security for the data pipeline.
Offers an interactive interface for visualizing and analyzing data in various formats, facilitating comprehensive insights and data-driven decisions.
The target user group for this database application includes:

Music enthusiasts seeking insights into their music preferences and behaviors.
Marketers aiming to understand trends and patterns in the music industry.
Researchers conducting studies on music-related topics.
Technical Description:
Dataset:
The data source for this project is real-time Spotify data accessed through their publicly available API. The data is retrieved in JSON format and contains information about tracks on the Spotify platform.

Normalized DynamoDB Tables:
The transformed data is stored in three normalized DynamoDB tables:

Album Table: Stores information about albums, including album ID, name, release date, total tracks, and artist ID (foreign key).
Artist Table: Stores information about artists, including artist ID, artist name, and external URL.
Song Table: Stores information about songs, including song ID, song name, duration in milliseconds, URL, popularity, song added date, album ID (foreign key), and artist ID (foreign key).
The normalization ensures data integrity and reduces redundancy, allowing efficient updates, deletions, and insertions.

Data Pipeline:
Extraction: AWS Lambda is used to extract data from the Spotify API in JSON format. The extraction process is scheduled to run weekly using an AWS CloudWatch event trigger. The extracted data is converted to CSV format and stored in an S3 bucket.
Transformation: AWS Lambda, triggered by AWS CloudWatch, transforms the CSV data into normalized tables suitable for efficient querying. The transformed data is stored in separate S3 buckets for each table.
Loading: Another AWS CloudWatch trigger activates the loading process, which loads the transformed data from S3 buckets into the normalized DynamoDB tables. The loading process is automated, ensuring up-to-date and accurate data in the database.
Visualization:
The data stored in DynamoDB is accessed through an AWS API Gateway, providing a secure and scalable method. The front-end of the application is developed using HTML, CSS, and JavaScript (React). Chart.js is used to visualize the data in various formats, including line charts, bar charts, and pie charts.

The project utilizes a combination of the following AWS services:

Front-End: HTML, CSS, JavaScript (React), Chart.js
Back-End: AWS Lambda, AWS CloudWatch, AWS API Gateway
Database: AWS S3, DynamoDB
HTML, CSS, and JavaScript (React) are used to build the user interface, while Chart.js facilitates data visualization. AWS Lambda handles data extraction and transformation, triggered by AWS CloudWatch events. AWS S3 is used for data storage and triggers transformation and loading processes. DynamoDB serves as the normalized database for efficient querying. AWS API Gateway provides secure access to the data stored in DynamoDB.

User Functionalities:
Accessing and Analyzing Spotify Data: The project allows users, including music enthusiasts, marketers, and researchers, to access and analyze Spotify data. This helps them gain insights into music trends, patterns, and behaviors.
Visualizing Data in Different Formats: The interactive interface provided by the project allows users to visualize and analyze data in various formats, such as line charts, bar charts, and pie charts. This facilitates comprehensive exploration of the data.
Building Scalable and Reliable Data Pipelines: The project demonstrates how AWS services can be utilized to build robust and efficient data pipelines that can be adapted to different industries and use cases. It serves as a blueprint for developers and organizations seeking to develop scalable and reliable data pipelines.
Conclusion:
The Spotify Data Pipeline and Visualization project showcases the utilization of AWS services to develop a secure, scalable, and efficient data pipeline for retrieving, transforming, and visualizing external data. The project enables users to access and analyze Spotify data, visualize it in various formats, and gain valuable insights into music preferences and behaviors. The project's implementation and architecture can serve as a foundation for building similar data pipelines in different domains and industries.




