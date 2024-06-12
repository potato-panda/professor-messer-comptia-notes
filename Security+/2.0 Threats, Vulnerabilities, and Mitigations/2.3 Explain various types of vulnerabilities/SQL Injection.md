### Code injection
- adding your own info into a data stream
### Enable because of bad programming
- the app should properly handle input and output
### So many different data types
- HTML, SQL, XML, LDAP, etc
### SQL - Structured Query Language
- the most common relationship db mgnt system language
### SQL injection (SQLi)
- put your own SQL requests into an existing app
- your app shouldn't allow this
### Can often be executed in a web browser
- inject in a form or field
# Building a SQL injection
### An example of website code:
```sql
"SELECT * FROM users WHERE name ='" + userName + "'";
```
### How it looks to the SQL database:
```sql
"SELECT * FROM users WHERE name ='Professor'";
```
### Add more info to the query:
```sql
"SELECT * FROM users WHERE name ='Professor' OR '1' = '1'";
%% OR '1' = '1' // will return table %%
```
### This could be very bad
- view all db info, delete db info, add users, DoS, etc...
