# Databricks – Practical Notes

Databricks provides:
- Managed Spark clusters
- Collaborative notebooks
- Delta Lake storage
- Job orchestration

## How I used Databricks in my project

- Created notebooks for ETL pipelines
- Read data from cloud storage
- Applied Spark transformations
- Stored output in Delta tables
- Scheduled jobs using Databricks Jobs

df = spark.read.csv("/data/input.csv", header=True)

clean_df = df.filter(df.age.isNotNull())

clean_df.write.format("delta").mode("overwrite").save("/data/output")

## Delta Lake

Delta Lake adds:
- ACID transactions
- Schema enforcement
- Time travel

Used for reliable data pipelines.

## Interview Notes

- Databricks is built on Spark
- Delta Lake provides reliability
- Clusters execute Spark jobs
- Notebooks are used for development

## official links to get started with Databricks:
## 📚 Free Databricks & Big Data Resources

### 📘 Official / Beginner Friendly
- 🔗 **[Databricks Free Training:](https://www.databricks.com/learn/training/home)**
- 🔗 **[Databricks Getting Started Docs:](https://docs.databricks.com/getting-started/index.html)** 
- 🔗 **[Databricks Community Edition (Free Workspace):](https://community.cloud.databricks.com)**

### 🎓 Structured Learning
- 🔗 **[Databricks Courses on Coursera:](https://www.coursera.org/courses?query=databricks)** 
- 🔗 **[YouTube Tutorials:](https://www.youtube.com/results?search_query=databricks+tutorial)**

### 📘 Related (Spark Basics)
- 🔗 **[Apache Spark Official Docs:](https://spark.apache.org/docs/latest/)**
