## XML Updater : a script to update xml files saved as blobs in database

#### 1. Add the files to Fix folder 
#### 2. Adjust the Database Details and the query according to the database you have
 db = pymysql.connect("Hostname","user","password","DBNAME" )
 sql_insert_blob_query = """UPDATE t_content SET data= %s WHERE t_content.iscurrent= %s AND t_content.ID = %s"""
 values = [pymysql.Binary(bin_data),1,name[:-4]]
#### 3. Execute the cells using Jupyter notebook 