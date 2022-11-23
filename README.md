# xetrapro


In the project I used Xetra dataset. Xetra stands for Exchange Electronic Trading and it is the trading platform of the Deutsche Börse Group. This dataset is derived near-time on a minute-by-minute basis from Deutsche Börse’s trading system and saved in an AWS S3 bucket available to the public for free.

The ETL Pipeline I created will extract the Xetra dataset from the AWS S3 source bucket on a scheduled basis, create a report using transformations and load the transformed data to another AWS S3 target bucket.

The pipeline deployed to  production environment that handle containerized applications. The production environment I write the ETL pipeline for consists of a GitHub Code repository, a DockerHub Image Repository, an execution platform such as Kubernetes and an Orchestration tool such as the container-native Kubernetes workflow engine Argo Workflows or Apache Airflow.
