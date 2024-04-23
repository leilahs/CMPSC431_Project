# CMPSC431_Project

**User's Manual**

<ins>Set-up instructions</ins><br />
<br />
<br />
<ins>Starting the program</ins><br />
<br />
On initial starts, the program will provide a list of types of commands that are available to you, the user. In order to select one, simply type the corresponding number in the CLI (Command Line Interface) and hit enter. Do not inlcude any characters other than the number and type it in number form, not letter. For example, type "1", not "one" or "1."<br />
<br />
<br />
<ins>Using specific commands</ins><br />
This section will break down the rules/guidelines specific to each command.<br />
<br />
1 . **Insert**<br />
<br />
The format of the sql query for an insert statement is INSERT INTO TableName (Column1, Column2, ...) VALUES (Value1, Value2, ...);<br />
The program will first prompt you for the table and columns you wish to change. You should type these in the following format...<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;TableName (Column1, Column2, ...)<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Ex: employees (id, name, department)<br />
<br />
Then you will be prompted for the values you wish to add. These should be in the following format...<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;(Value1, Value2, ...), (Value1, Value2, ...), ...<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Ex: (5392, 'John', 'Sales'), (1234, 'Jane', 'Finance')<br />
<br />
After entering the values, the program will output a number corresponding to the number of rows that have been added in your chosen table.<br />
<br />
<br />
2. **Delete**<br />
<br />
The format of the sql query for a delete statement is DELETE FROM TableName WHERE Condition;<br />
The program will first prompt you for the table you wish to delete from. You should type this in the following format...<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;TableName<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Ex: employees<br />
<br />
Then you will be prompted for the condition which determines exactly which rows will be deleted. This should be in the following format...<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;column = value<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Ex: id = 1234<br />
<br />
After entering the condition, the program will output a number corresponding to the number of rows that have been deleted in your chosen table.<br />
<br />
<br />
3. **Update**<br />
<br />
The format of the sql query for an update statement is UPDATE TableName SET Column1 = NewValue WHERE Condition;<br />
The program will first prompt you for the table you wish to delete from. You should type this in the following format...<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;TableName<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Ex: employees<br />
<br />
The second prompt will be for what column(s) you want to change and what you want to change it(them) to. This should be in the following format...<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;column = value<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Ex: department = 'Marketing'<br />
<br />
Lastly you will be prompted for the condition which determines exactly which rows will be changed. This should be in the following format...<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;column = value<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Ex: id = 5392<br />
<br />
After entering the condition, the program will output a number corresponding to the number of rows that have been updated in your chosen table.<br />
<br />
<br />
4. **Search**<br />
<br />
The format of the sql query for a delete statement is SELECT Column1, Column2, ... FROM TableName1, TableName2, ... WHERE Condition;<br />
The program will first prompt you for what column(s) you want to change and what you want to change it(them) to. If you wish to select all columns from the given table(s), simply use '*'. This should be in the following format...<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Column1, Column2, ...<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Ex: id, name<br />
<br />
The second prompt will be for the table(s) you wish to search in. If you chose more than one table, the query will create a temporary table of the form table1 X table2 which it will then search in. Additionally, if there are column names that are the same between multiple tables, use the format TableName.ColumnName to specify which one you are referring to. You should type this in the following format...<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;TableName1, TableName2, ...<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Ex: employees, departments<br />
<br />
Then you will be prompted for the condition which determines exactly which rows will be deleted. This should be in the following format...<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ColumnName = value<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Ex: employees.id = 1234<br />
<br />
After entering the condition, the program will output the selected rows.<br />
