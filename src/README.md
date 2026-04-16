
# Chicago taxi fares ETL project

This project was implemented as part of the Cubix Technology of Education 21-week Data Engineer course. The codes are the intellectual property of my instructor Balázs Balogh. Their use can only be done with his permission. During the course, this project served to demonstrate how to automatically provide clean, interpretable data for Data Analysts from a source data.










## In this section, I will explain the main role of each file in the src directory and what role it plays in the project.

- 01_hw_week7.ipynb:
As a warm-up, the homework was to process a JSON source. This is what is included in this notebook.

- 02_web_scraping.ipynb:
The Pickup Community Area and Dropoff Community Area columns of the source data only contained numeric values. To make it easier to understand where a taxi trip went from and went to, we made a dimension table to be able to expand the source data with the names associated with this data. To do this we were scraping the following web page:
"https://en.wikipedia.org/wiki/Community_areas_in_Chicago"
At the end of the notebook, we created the community_areas_master.csv file from the Community data extracted from the html.

- 03_get_taxi_data.ipynb:
In this notebook, we first read the daily taxi fare data for a period, and then, as an important initial element of the ETL process, we created the read that performs the data for one day.

- 04_get_weather_data.ipynb:
As the next important initial element of the ETL process, we created the retrieval of weather data for a given day.

- 05_date_dimension.ipynb:
In this notebook, we created a dimension table of the days of the year corresponding to the source data with the day_of_week, is_weekend data to make further data analysis work easier.

- 06_taxi_data_mapping.ipynb:
In this file, after transforming the source data, we created the important but still missing dimension tables and merged them with the source data.

- 07_transform_load.ipynb:
In this file we set up the basic code for the Transform Load Lambda function which we will use on our Amazone Web Services
account.

- 08_extract_lambda_function.ipynb:
Now we moved our Exract code to the AWS Lambda function to make extracting data an automated process.

- 09_transform_load_lambda_function.ipynb:
In this part we set the needed functions in AWS Lambda so these functions will be also automated.

- 10_hw_week11.ipynb:
In this homework we gave a sample of what kind of queries can a Data Analyst make in AWS Athena on our dataset.

- 11_create_datamodel.ipynb:
As a final step we read our S3 Bucket's data and prepare it so that we can make further Data analysis steps if needed.



## License

The codes are the intellectual property of my instructor Balázs Balogh. Their use can only be done with his permission. Please contact him to get the needed permissions: balazs.balogh@cubixedu.com Thank you, that you using this legal way.


## Appendix

In this part I want to thank my instructor that I could be part of this project.

