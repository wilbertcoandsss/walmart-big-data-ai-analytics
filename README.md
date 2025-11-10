# Walmart Big Data & AI Visualizations

The group-project for Big Data Analytics, one of my courses in my Master's School. In this project, we built a distributed big-data analytics pipeline for Walmart using Apache Hadoop and its environment in Cloudera Quickstart VM. 

We designed and Implemented an end-to-end big data architecture based on Apache Hadoop ecosystem, together with another integrated services, such as: Apache Kafka, Apache Spark (including MLLib), Hive (Structured SQL-engine above HDFS), MongoDB, Neo4J Graph Analytics, and ViteJS & ExpressJS for both frontend visualization and backend services. We also deploying an CronJob to ensure periodic refresh for data training model and data ingestion.

Main Features for this Project includes:
- Machine Learning & Analytics, trained two models to do both customer segmentation and churn classification.  KMeans Clustering to do customer segmentation, based on their behavior and three supervised model (Linear Regression, Decision Tree, and Random Forest) to predict customer churn. Exposed via Flask API so the data can be consumed on visualization layers on frontend.
- Data Streaming, using Apache Kafka as a message broker for real-time customer transaction data and log (such as login, chat, register, item added to cart, and many more), coordinated via Zookeeper in Hadoop for distributed cluster management and MongoDB for semi-structured dataset.
- Graph Intelligence, built using Neo4J Graph Database to model relationships between customers, products, and transactions, enabling graph-based recommendations and visualizations.
- Interactive Dashboard, developed a ViteJS based analytics with ExpressJS on the backend to subscribing to Kafka Consumer.

All of those technologies resulting in real-time transaction streaming, product recommendation, and interactive both dashboard and graph visualization to deliver actionable insights from a large-scale customer and sales data, both in real-time or batch data processing.
