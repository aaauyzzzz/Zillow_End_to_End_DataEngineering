  This is the Zillow end-to-end data engineering project. 

![data_pipeline](https://github.com/user-attachments/assets/7ad8fbf8-c6a9-420e-afbf-4845c895b7fd)

  In this data engineering project, I built and automated a python ETL process that would extract real estate properties data from Zillow Rapid API (https://rapidapi.com/s.mahmoud97/api/zillow56/playground/apiendpoint_444379e9-126c-4fd2-b584-1c9c355e3d8f), loaded it into amazon s3 bucket which then triggers a series of lambda functions which then ultimately transformed the data, converted into a csv file format and loaded the data into another S3 bucket using Apache Airflow. Apache airflow will utilize an S3KeySensor operator to monitor if the transformed data has been uploaded into the aws S3 bucket before attempting to load the data into an amazon redshift. 

  After the data was loaded into aws redshift, then I connected amazon quicksight to the redshift cluster to visualize the Zillow data.

  This project will entirely be carried out on AWS cloud platform.

  Thanks to @tuplespectra (https://www.youtube.com/watch?v=j_skupZ3zw0&t=146s) for guiding
