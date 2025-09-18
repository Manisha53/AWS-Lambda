# AWS-Lambda
An object or file organizer project based on date using AWS lambda - A Python execution

We’re going to write our Python script that will create a folder in the S3 bucket we created. The folder will be named based on the day we create the folder. Afterwards, our Python script will also move all the files that someone uploads into our S3 bucket in the folder based on the day the file was uploaded.

We only need 2 modules for this project. The first module is Boto3. Whenever you’re using Python to create resources in AWS, you always have to import the Boto3 module. The second module that we will import is datetime — According to the company problem, we have to create a folder in our S3 bucket and we will name that folder based on the day the file was uploaded into our S3 bucket. Therefore, in order to be able to name our folder based on the day, we have to import the module datetime.
