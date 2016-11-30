#aws-dynamodb-iot Raspberry Pi Tempreture data visualisation

## Synopsis

Simple scripts to **publish** and **query** AWS DynamoDB database that contains time-series of data sent by our Raspberry Pi. The data is represented as a line plot.

## About Code

index.html - simple front-end for query of DynamoDB and data processing
table_processor.js - processing of the query data and representation as HTML table using dynatable.js
plotly_scatter.js - visualization of the processed data with plot.ly JavaScript library
publish_code.py - publishes data to dynamoDB database in aws

## Installation

Provide the location of your aws iot thing certificates in script and change your data you want to send in script.

Then run publish_code.py script:

python publish_code.py

The code should work out of the box, just copy all files into the same directrory. 
You have to obtain security credentials using AWS IAM, make sure they allow you to read DynamoDB, and have the databas(es) set-up as described in posts mentioned above.

Just open index.html page to check whether your values are published in your dynamoDB database.

## Contributors
95subodh
Feel free to contact me incase of any issues

## License

MIT
