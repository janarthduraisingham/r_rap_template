The code folder should contain all code e.g .R, .py, .sql scripts

The data folder should contain all external data e.g. postcode to MSOA lookup

The intermediate folder should contain all intermediate datafiles ingested in scripts e.g. a SQL extraction dataset that then gets ingested into R/Python

The output folder should contain all outputs e.g. .png plots

You should ensure no data gets committed the repository - this is to avoid the risk of personal data being pushed to the remote repo, and to minimise the size of the repo. The .gitignore will help to avoid committing common datafile types such as .xlsx, .csv, but you should always run "git status" before committing so you are aware what is being tracked. You can add necessary exceptions to the .gitignore by adding the "folder/filename" path to it, preceded with an exclamation mark, !