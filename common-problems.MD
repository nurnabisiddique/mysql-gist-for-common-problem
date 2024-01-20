1. MySQL: Error Code: 1118 Row size too large (> 8126). Changing some columns to TEXT or BLOB 

For MariaDB users (version >= 10.2.2) and MySQL (version >= 5.7), the simple solution is:

ALTER TABLE `table` ROW_FORMAT=DYNAMIC;

