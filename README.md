# AWSGlueCrawler
AWS Glue Crawler Demo
1.	Create an S3 bucket and upload the customer and orders csv files in newly created bucket
   ![image](https://github.com/user-attachments/assets/c3d3633a-2e0b-4eeb-9a5d-f0f66f923cff)
  
2.	Goto AWS Glue  Database Catalog  Databases  Add Database
   ![image](https://github.com/user-attachments/assets/beb29bf0-b6e5-4802-89c9-33782932e213)

3.	Click on Add Tables Using Crawler
   ![image](https://github.com/user-attachments/assets/533468d7-a127-4aa5-9b48-a624314d8151)

4.	Add data source
  	![image](https://github.com/user-attachments/assets/74a68297-e39a-4622-a3dc-61df94d68de1)
    ![image](https://github.com/user-attachments/assets/93aaed54-7973-4561-a16d-d0f1fb3dbd2c)

5.	Create new IAM Role to allow AWS Glue service to read file from S3
    ![image](https://github.com/user-attachments/assets/97d9daf8-139e-4b82-9909-64f4604eabda)

6.	Click on View Role to ensure correct access is provided to S3 bucket
    ![image](https://github.com/user-attachments/assets/5f839030-b8c2-4286-8726-4348cb2a6960)

7.	Next; select database. Table prefix (optional), crawler schedule
    ![image](https://github.com/user-attachments/assets/ccb317ee-d24e-4a10-a8d2-56f8398b5af8)

8.	Review the properties and click Create Crawler
    ![image](https://github.com/user-attachments/assets/17c3451e-9c50-4b40-ae71-eb8814238e30)
    ![image](https://github.com/user-attachments/assets/e96640c6-f747-4cb7-a74c-d1a7bb95507c)

9.	Click on Run Crawler to start
    ![image](https://github.com/user-attachments/assets/f7b83d94-ea9d-4bf4-bd64-62d4bfb83ba7)

10.	Check the status of Crawler
    ![image](https://github.com/user-attachments/assets/04dba218-0917-495b-9301-d20a70d550b9)

11.	Check the tables created in database (after successful completion of crawler execution)
    ![image](https://github.com/user-attachments/assets/274390bf-878e-4699-92a2-36cb76a81b37)

12.	We can edit the table schema to remove any column, rename any column etc. This will not remove actual data from CSV files
    ![image](https://github.com/user-attachments/assets/6565a080-058e-4e25-85e8-504b0d7e9b86)

## Acknowledgements

This project was developed based on the concepts and examples provided in the Udemy course "[Data Engineering on AWS - The complete training](https://www.udemy.com/course/data-engineering-on-aws/)" by [Ashish Prajapati]
