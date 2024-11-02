# Cloud-
Genai study jams
Pub/Sub is a messaging service for exchanging event data among applications and services.
A producer of data publishes messages to a Pub/Sub topic. A consumer creates a subscription to that topic. 
**A topic acts like a channel or a stream where messages are published. Producers send messages to a specific topic instead of directly to a consumer.


Subscribers either pull messages from a subscription or are configured as webhooks for push subscriptions. 
*1. Pull Subscription
How it Works: With a pull subscription, the subscriber explicitly requests (or "pulls") messages from the Pub/Sub server 
whenever it's ready to process them. This involves the subscriber making API calls periodically or on-demand to retrieve any new messages from the subscription.

Every subscriber must acknowledge each message within a configurable window of time.


What I  learnt
Set up a topic to hold data.
Subscribe to a topic to access the data.
Publish and then consume messages with a pull subscriber.



CLOUD SCHEDULER

Alright! Imagine you have a robot assistant, and this robot can be told to do certain tasks, like ring a bell, fetch something, or turn on a light. Now, you want this robot to automatically ring a bell at 8 AM every morning without you having to tell it each time.

In the same way, Cloud Scheduler is like the robot that can do tasks automatically on a schedule. But Cloud Scheduler needs to know what kind of task you want it to do. This is where Target Type comes in.

When you choose Target Type: HTTP in Cloud Scheduler, you’re saying, "I want you to send an online message to a specific address (like a website link) that is ready to listen and do something when it gets the message."

So, picking HTTP is like telling your robot, “Every morning, go to the bell’s location and push it at 8 AM.” Cloud Scheduler’s “HTTP target” sends this “push” message to a specific online address (like a Cloud Function) that does the task on schedule.



Overview
Cloud Scheduler lets you set up scheduled units of work to be executed at defined times or regular intervals. These work units are commonly known as cron jobs. Typical use cases might include sending out a report email on a daily basis, updating cached data every 10 minutes, or updating summary information once an hour. You can automate everything, including retries in case of failure to reduce manual intervention.

Each cron job created using Cloud Scheduler is sent to a target, where the work for the task is accomplished. The target must be one of the following types:

Publicly available HTTP/S endpoints
Pub/Sub topics
App Engine HTTP/S applications
In this lab you will learn how to:

Create a Cloud Scheduler job.
Set a recurring schedule for a job.
Specify a Cloud Pub/Sub topic as the job target.
Run a job.
Verify success.











A Cloud Run function is a piece of code that runs in response to an event, such as an HTTP request, a message from a messaging service, or a file upload. Cloud events are things that happen in your cloud environment. These might be things like changes to data in a database, files added to a storage system, or a new virtual machine instance being created.

Since Cloud Run functions are event-driven, they only run when something happens. This makes them a good choice for tasks that need to be done quickly or that don't need to be running all the time.

For example, you can use a Cloud Run function to:

automatically generate thumbnails for images that are uploaded to Cloud Storage.
send a notification to a user's phone when a new message is received in Pub/Sub.
process data from a Cloud Firestore database and generate a report.
You can write your code in any language that supports Node.js, and you can deploy your code to the cloud with a few clicks. Once your Cloud Run function is deployed, it will automatically start running in response to events.

This hands-on lab shows you how to create, deploy, and test a Cloud Run function using the Google Cloud console.

What you'll do
Create a Cloud Run function
Deploy and test the function
View logs



