# Creating a Streaming Data Pipeline for a Real-Time Dashboard with Dataflow

# Overview
- **In this Project, am working to improve the company that owns a fleet in New York City a taxi cabs and are looking to monitor how well their business is doing in real-time. i will build a streaming data pipeline to capture taxi revenue, passenger count, ride status, and much more, and then visualize the results in a management dashboard.**

##### I will build a streaming data pipeline to monitor sensor data, and then visualize the dataset through a dashboard.

I practiced: 
- By Creating a Dataflow job from a pre-existing template and subscribing to a Pub/Sub topic. 
- Streaming and monitoring a Dataflow pipeline into BigQuery and Analyzing results with SQL, and Visualizing key metrics in Data Studio. 
- Please note that,I Used Strong SQL commands required. 
- I will explored BigQuery in more details.

### Task 1. create the taxi_rides dataset or table as in Bigquery
- I Sourced for a pre-created Pub/Sub topic and create a BigQuery dataset
In this task, I created the taxirides dataset. I have two different options which you can use to create this, using the ``Google Cloud Shell`` or ``the Google Cloud Console``.

- ``Pub/Sub`` is an asynchronous global messaging service. By decoupling senders and receivers, it allows for secure and highly available communication between independently written applications. Pub/Sub delivers low-latency, durable messaging.

- In Pub/Sub, publisher applications and subscriber applications connect with one another through the use of a shared string called a topic. A publisher application creates and sends messages to a topic. Subscriber applications create a subscription to a topic to receive messages from it.

- Google maintains a few public Pub/Sub streaming data topics for labs like this one. We'll be using an extract of the ``NYC Taxi & Limousine Commission’s open dataset``. The Pub/Sub topic has already been created and populated in your project environment.

BigQuery is a serverless data warehouse. Tables in BigQuery are organized into datasets. In this project, messages published into Pub/Sub will be aggregated and stored in BigQuery.

### Task 2. Create a Cloud Storage bucket
- In this task, I created a Cloud Storage bucket to provide working space for your Dataflow pipeline.

- Cloud Storage allows world-wide storage and retrieval of any amount of data at any time. I can use Cloud Storage for a range of scenarios including serving website content, storing data for archival and disaster recovery, or distributing large data objects to users via direct download.

### Task 3. Set up a Dataflow Pipeline
- In this task, I set up a streaming data pipeline to read sensor data from Pub/Sub, compute the maximum temperature within a time window, and write this out to BigQuery.

- Dataflow is a serverless way to carry out data analysis.
