# Consumer Financial Protection Bureau Data Engineering Project

## This is an end-to-end data engineering project that extracts data from the Consumer Financial Protection Bureau (CFPB) API, transforms it using PySpark, and loads it into DynamoDB. The data goes through the following flow:

### Web_API > MongoDB (Atlas Cloud) > AWS EventBridge > Lambda > S3 > Glue > DynamoDB

#### Requirements
To run this project, you'll need:

- Python 3.7 or higher
- An AWS account with permissions to use EventBridge, Lambda, S3, Glue, and DynamoDB
- A MongoDB Atlas account and cluster
- An API key for the CFPB API
 
#### Installation
1. Clone this repository:

git clone https://github.com/your_username/cfpb-data-engineering.git


2. Install the required Python libraries:

pip install -r requirements.txt

3. Set up your AWS credentials by following the official documentation.

4. Set up your MongoDB Atlas credentials by following the official documentation.

5. Create a .env file with the following environment variables:

CFPB_API_KEY=your_api_key
MONGODB_URI=your_mongodb_uri
S3_BUCKET_NAME=your_s3_bucket_name

#### Usage
Run the etl.py script to extract data from the CFPB API, transform it using PySpark, and load it into DynamoDB:


python etl.py

Alternatively, you can run the extract.py, transform.py, and load.py scripts separately if you want more control over the individual steps.

#### Credits
This project was created by Zia.
