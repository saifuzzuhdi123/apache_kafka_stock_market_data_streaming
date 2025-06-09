# Apache Kafka Stock Market Data Streaming

This project focused on real-time stock market data streaming using Apache Kafka. The project demonstrates how to use Apache Kafka for capturing, processing, and streaming stock market data efficiently. It is implemented entirely in Jupyter Notebook, making it easy to follow along with the code, explanations and deployed in Amazon EC2 instance and S3 . The repository is ideal for those interested in learning about real-time data pipelines, stream processing, and practical applications of Kafka in the context of financial data.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Project Structure](#project-structure)
- [Requirements](#requirements)
- [Setup Instructions](#setup-instructions)
- [Usage](#usage)
- [Acknowledgements](#acknowledgements)

## Overview

This repository showcases how Apache Kafka can be used to stream stock market data in real time. The project covers:

- Setting up Kafka producers and consumers
- Simulating stock market data streams
- Real-time data processing using Jupyter Notebook in AWS 

## Features

- Real-time data streaming with Apache Kafka
- Utilised Amazon AWS EC2, S3, Athena, Glue, Crawler to deploy in cloud
- Stock market data simulation or integration with real APIs
- Interactive data exploration and visualization in Jupyter Notebook
- End-to-end example for learning Kafka in the context of finance

## Project Structure

```
.
├── assets/
│   └── project_architecture.jpg
├── data/
│   └── <Sample or generated data>
├── notebooks/
│   └── <Jupyter Notebooks for Kafka Producer and Consumer>
├── scripts/
│   └── kafka_EC2_setup.txt
└── README.md
```

## Requirements

- Python 3.7+
- Jupyter Notebook
- Apache Kafka (local or remote cluster)
- Python libraries (see `requirements.txt`):
  - kafka-python
  - pandas
  - matplotlib
  - numpy

## Setup Instructions

1. **Clone the repository:**
   ```bash
   git clone https://github.com/pavithra19/apache_kafka_stock_market_data_streaming.git
   cd apache_kafka_stock_market_data_streaming
   ```

2. **Install dependencies in Jupyter Notebook:**
   ```bash
   pip install kafka-python
   ```

3. **Start Apache Kafka:**
   - Download and install Apache Kafka in EC2 instance, check the kafka_EC2_setup file inside scripts folder.
   - Start Zookeeper and Kafka server:
     ```bash
     # Start Zookeeper
     bin/zookeeper-server-start.sh config/zookeeper.properties
     # Start Kafka server
     bin/kafka-server-start.sh config/server.properties
     ```

4. **Run the Jupyter Notebook:**
   ```bash
   jupyter notebook
   ```
   - Open the provided notebook(s) and follow the instructions.

## Usage

- The provided Jupyter Notebooks walk you through producing and consuming stock market data streams.
- You can simulate data or connect to a real-time data API.
- Visualize and analyze data streams in real time.

## Acknowledgements

- [Apache Kafka](https://kafka.apache.org/)
- [Jupyter Project](https://jupyter.org/)
