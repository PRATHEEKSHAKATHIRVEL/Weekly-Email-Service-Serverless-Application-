# Weekly-Email-Service-Serverless-Application-
This project demonstrates a serverless email service using AWS. It enables sending automated emails by integration of AWS services.
AWS SERVICES USED 
1.IAM Policies - Helps in granting permissions to Lmbda functions and services
2.AWS SES (Simple Email Service) - Sends emails to verified domains/adresses
3.AWS LAMBDA - Helps in reading data from S3, formats the email, and calls SES to send
4.S3 - Used for storage purposes
5.Amazon Event Bridge Scheduler - Helps in scheduling emails at specific times like weekly, daily
SETUP STEPS 
1.Create an S3 bucket with unique bucket name and upload email templates, contacts file.
2.Verify Emails in SES ( Here I have verified email addresses and not domain names. You can verify from and to addresses and create identies)
3.You can also send test mails from verified identies.
4.Create a lambda function to send weekly or daily mails by using appropriate python code.
5.You can also test the function manually before using event scheduler.
6.Create policies allowing S3, SES  access and attach to Lambda.
7.Set Event Bridge Scheduler and set target as Lambda function.
8.So, when Lambda is triggered the mail can be sent 

