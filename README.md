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

All options on sqlmap page
https://github.com/sqlmapproject/sqlmap/wiki/Usage
