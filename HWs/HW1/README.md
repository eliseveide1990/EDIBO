uzdevuma apraksts : Analysis of Windows event logs using PANDAS DataFrame  

How do I find Windows event log?
To view events:

    Click Start, point to Programs, point to Administrative Tools, and then click Event Viewer.
    In the console tree, right-click the appropriate log file. ...
    Click a specific event in the details pane to display the Event Properties dialog box and details about the event.
    
    talak nesaprotu 
    
    Python | Pandas DataFrame. Pandas DataFrame ir divdimensiju mainīga lieluma, potenciāli neviendabīga tabulas datu struktūra ar marķētām asīm (rindām un kolonnām). Datu rāmis ir divdimensiju datu struktūra, t.i., dati ir izlīdzināti tabulas veidā rindās un kolonnās.
    
    content_size_summary_df = logs_df.describe(['content_size'])
content_size_summary_df.toPandas() 

Kā alternatīvu mēs varam izmantot SQL, lai tieši aprēķinātu šo statistiku. Modulim pyspark.sql.functions ir daudz noderīgu funkciju, lai uzzinātu vairāk, skatiet dokumentāciju. 

After we apply the .agg() function, we call toPandas() to extract and convert the result into a pandas DataFrame, which offers better formatting on Jupyter Notebook

 Selecting a single row

In order to select a single row using .iloc[], we can pass a single integer to .iloc[] function.
import pandas as pd
 
# making data frame from csv file
data = pd.read_csv("nba.csv", index_col ="Name")
 
 
# retrieving rows by iloc method 
row2 = data.iloc[3] 
 
