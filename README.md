# Shell Commands

1. Find file in a directory

  ```
  find <directory> -name "<file name>"
  find <directory> -regex "<regex>"
  ```
2. Search file by keyword/regex

  ```
  grep -R "<keyword>" <directory>
  ``` 
3. Retrieve matching text in a file
  
  ```
  grep -oEi '<regex>' <directory>
  ```
4. Join multiple lines into one line with delimeter
  
  ```
  <source of multiple lines> | paste -s -d "<delimiter>"
  <source of multiple lines> | perl -pe 's/\n$/ <delimeter text> /'
  ```
5. Curl with HTTP authentication

  ```
  curl -u <username>:<password> <url>
  ```
6. To redirect both `STDOUT` and `STDERR` to the same place, use the `>&` symbol. To redirect `STDOUT` only, use `1>`. Toredirect `STDERR` only, use `2>`.