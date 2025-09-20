📂 AWS Lambda – S3 Object Organizer

A serverless file organization project that automatically creates date-based folders in Amazon S3 and moves uploaded files into them using an AWS Lambda function written in Python.

🚀 Overview

This project demonstrates how to use AWS Lambda with Python (Boto3) to automatically organize files uploaded to an S3 bucket:

Creates a folder named after the current date inside the S3 bucket.

Moves any newly uploaded file into the corresponding date-based folder.

Eliminates manual organization tasks.

🛠️ Technologies Used

AWS Lambda – Serverless compute

Amazon S3 – Object storage

Python 3.x

Boto3 – AWS SDK for Python

datetime – To generate date-based folder names

⚙️ How It Works

An S3 bucket (already created) receives file uploads.

An S3 Event Notification triggers the AWS Lambda function.

The Lambda function:

Checks the upload date.

Creates a folder in the bucket named with that date (if not present).

Moves the uploaded file into the corresponding folder.

📋 Prerequisites

An AWS account with permissions to create S3 buckets and Lambda functions.

An existing S3 bucket.

Python 3.x installed locally (for development).

Boto3 installed:

pip install boto3

▶️ Deployment Steps

Create / choose an S3 bucket.

Create an AWS Lambda function in Python 3.x.

Upload the s3-object-organizer.py script as the Lambda code.

Configure an S3 Event Notification (Object Created) to trigger the Lambda.

Test by uploading files to the S3 bucket — they should be automatically moved into date-based folders.

📝 Example Folder Structure
my-s3-bucket/
  2025-09-18/
    file1.jpg
    file2.pdf
  2025-09-19/
    file3.png

📚 Modules Used

Boto3 – To interact with S3 from Python.

datetime – To generate date strings for folder names.

✨ Features

Event-driven & serverless (no servers to manage).

Fully automated file organization.

Simple to deploy and extend.
