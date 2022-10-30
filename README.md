# Creating a Streaming Data Pipeline for a Real-Time Dashboard with Dataflow

# Overview
- In this Project, a company that owns a fleet of New York City taxi cabs and are looking to monitor how well their business is doing in real-time. i will build a streaming data pipeline to capture taxi revenue, passenger count, ride status, and much more, and then visualize the results in a management dashboard.

### Task 1. 
- I Sourced for a pre-created Pub/Sub topic and create a BigQuery dataset
In this task, I created the taxirides dataset. I have two different options which you can use to create this, using the ``Google Cloud Shell`` or ``the Google Cloud Console``.

- ``Pub/Sub`` is an asynchronous global messaging service. By decoupling senders and receivers, it allows for secure and highly available communication between independently written applications. Pub/Sub delivers low-latency, durable messaging.

- In Pub/Sub, publisher applications and subscriber applications connect with one another through the use of a shared string called a topic. A publisher application creates and sends messages to a topic. Subscriber applications create a subscription to a topic to receive messages from it.

- Google maintains a few public Pub/Sub streaming data topics for labs like this one. We'll be using an extract of the ``NYC Taxi & Limousine Commission’s open dataset``. The Pub/Sub topic has already been created and populated in your project environment.

BigQuery is a serverless data warehouse. Tables in BigQuery are organized into datasets. In this project, messages published into Pub/Sub will be aggregated and stored in BigQuery.
