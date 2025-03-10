# mongodb-pyspark-docker
This repository demonstrates the integration of MongoDB with PySpark. It provides a step-by-step guide on how to set up MongoDB locally using Docker Compose, insert sample data, and perform transformations using PySpark.

# MongoDB with Mongo Express & PySpark Integration

This project sets up a MongoDB database along with Mongo Express (a web-based admin interface for MongoDB) using Docker Compose. It also includes a PySpark Jupyter Notebook to interact with MongoDB.

## 📌 Features:
    -   MongoDB setup using Docker and docker-compose
    -   JDBC connection for PySpark
    -   Example table creation using mongo express
    -   Data insertion using pymongo and retrieval using PySpark
    -   Data transformation using PySpark
    -   Data load into mongodb using PySpark
    -   Steps to install dependencies and configure the setup

## 🛠️ Tech Stack
    - **ETL Tools**: PySpark
    - **Database**: mongoDB and mongo express
    - **Language**: Python
    - **Container**: Docker

## Prerequisites

Ensure you have the following installed on your system:

    -   Docker
    -   Python (Recommended: Python 3.13.1)
    -   Jupyter Notebook (Optional, if running manually)
    -   PySpark

## 🚀 Setup Instructions

1) Clone the repository

``` bash
    git clone https://github.com/ItisVenkatesh/mongodb-pyspark-docker.git
    cd mongo-pyspark-docker
```
2) Run Docker and start containers

After starting Docker engine,

``` bash
    docker-compose up --build -d
```
This will,
    -   Start MongoDB on port 27017
    -   Start Mongo Express on port 8081

3) Mongo Express

Open the URL [http://localhost:8081](http://localhost:8081) in your browser.

Log in using below credentials.
username: admin
password: pass

Explore the created mongodb using mongo express UI.

4) Install dependencies

``` bash
    pip install -r requirements.txt
```

5) Explore the Notebook

    -   Open notebook file "mongodb_pyspark.ipynb" under "notebooks" folder.
    -   Explore the notebook by running the cells from beginning.
    -   The sample data can be inserted at the top cell using pymongo. 
    -   Feel free to modify the cells and explore.

6) Stop docker container

Once done, use below command to stop docker container

``` bash
    docker-compose down
```    

## License

This project is licensed under the MIT License - see the LICENSE file for details.
