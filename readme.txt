DataWeekender2022 Repo - contians Data and Presentation in .pdf file.

Demo divided into 2 seprate Repos
1.Repo has only ADF
     https://github.com/alpaBuddhabhatti/DataWeekender2022_ADF
2.Repo has Azure Function and ARM template for Azure Logic Apps and Azure SQL Server with DB.
     https://github.com/alpaBuddhabhatti/DataWeekender2022_CU5
     
     
 There are rwo Demos.
 
Demo1 - Moving File from Azure blob to Azure SQL Server + Generating Manifest file(using Azure Function) + Sending Email (ADF)
 
         Here , ADF - ADF_AF_ALA_Demo1 pipleine
                Data - .csv files in blob storage - file-in
                
Demo2 - Move csv file to Azure SQl Server, Move .jpg files to blob input container, sending email uisng logic Apps
        Here, Azure Function is using Azure Function with Blob trigger and Bloboutput bindings. So its not directly involved. However, its looking blob input container and as soon as file appeares into this container, small peace of code/Resizing email.
        Here , ADF - ADF_AF_ALA_Demo2 pipleine
                Data - .csv files in blob storage - file-in
                 Car.csv file + .jpg files.
        
  
  Following steps need to performs.
  1. Azure Blob storage with 3 contianers 
       1. file-in  - Also upload 3 .csv files before run pipeline demo1
       2. input    - 
       3. output 
       
   2. Azure SQL Server  - this can be created using ARM tempalte  (you can find in second repo mentioned as above)
   3. Azure Logic Apps  - This can be created using ARM tempalte  (you can find in second repo mentioned as above)
   4. Azure Functions   - This can be created using ARM temapltes (you can find in second repo mentioned as above)
                
     
