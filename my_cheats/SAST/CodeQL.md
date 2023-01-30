# CodeQL
#plateform/multiple #target/local #cat/CODE/WHITEBOX #tag/CodeQL


## CodeQL - create database
Create CodeQL database for a project in the current directory.
https://codeql.github.com/docs/codeql-cli/creating-codeql-databases/
```
codeql database create <database-name> --languages <programming-language> --source-path . 
```

## CodeQL - create database
Command to run predefined Java security queries, package to run.
ex package for java security queries: codeql/java-queries@0.5.0:Security/CWE
https://codeql.github.com/docs/codeql-cli/manual/database-run-queries/
```
codeql database run-queries -- <database-dir> <package-name>
```

## CodeQL - interpret query results
To interpret the result of `run-queries` sub-command to a human readable format.
https://codeql.github.com/docs/codeql-cli/manual/database-interpret-results/
```
codeql database interpret-results --output=interpret-result.csv --format=csv   -- <database-dir>/
```

## CodeQL - decode BQRS file
To decode the BQRS result file
https://codeql.github.com/docs/codeql-cli/manual/bqrs-decode/  


```
codeql bqrs decode <path-bqrs-file> --entities=all
```