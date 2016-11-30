aws-dynamodb-iot Raspberry Pi Tempreture 

IoT button data visualization

Simple scripts to query AWS DynamoDB database that contains time-series of data sent by our Raspberry Pi. The data is represented as a line plot.

About files in this repository:
index.html - simple front-end for query of DynamoDB and data processing
table_processor.js - processing of the query data and representation as HTML table using dynatable.js
plotly_scatter.js - visualization of the processed data with plot.ly JavaScript library
The code should work out of the box, just copy all three file into the same directrory. The script is also hosted online here. 
You have to obtain security credentials using AWS IAM, make sure they allow you to read DynamoDB, and have the databas(es) set-up as described in posts mentioned above.
