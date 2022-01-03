# egenproject3
# Creating a pipeline using DATA FUSION
# PROJECT:
In this project I built and created a data pipeline graph with data fusion. I used wrangler and data pipeline features in cloud data fusion to clean to transform and to process eccentric data. So first I connected cloud data fusion to couple of data source to apply basic transformation and then join to data sources and write data to a sync.

# Architecture
![image](https://user-images.githubusercontent.com/28685243/147948363-14d5fd0b-271d-4b04-bf4c-08a9bf4c3896.png)

## DATA FUSION:

It’s a data integration service using this service we can easily map and build and test complex data pipelines. Extracting transforming and loading data of any size structure or source can be done.  

## PROJECT PROCESS: 

For the initial setup activated could fusion API. Created an instance with project name and then in IAM ADMIN added a member which is the service account that I had created and give it the role could data fusion API service agent. Then created a bucket with the project name and saved the file taxi sample csv. Created a temp folder along with this bucket. Then went into big-query and created a dataset got selective data from the data we have in the bucket. Now as the base is setup now, I went into cloud fusion and from that went to view instance to get access to wrangler and other options. I used wrangler for this project as wrangler it has a pre-configured connection that we can go ahead and pick. Over all it gives a snapshot of transformation and result.  So, once I when into wrangler opened the data that is in the bucket, I created earlier did some transformations and cleaning then created a batch pipeline. In batch pipeline I was connected GCS file to wrangler got the big-query table which I have saved earlier then added a joiner and added both wrangler and big-query and which connecting to another big-query once it deployed, I ran the process.

![image](https://user-images.githubusercontent.com/28685243/147948381-2581c4c4-b03f-4192-9600-45ff8b840d37.png)

Then I was able to see the joined table in big query dataset with a new table. 
