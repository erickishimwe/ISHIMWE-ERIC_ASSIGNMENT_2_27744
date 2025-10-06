# Question 1: Create Pluggable Database (PDB)

Description:
This project demonstrates how to create a Pluggable Database (PDB) in Oracle from the PDB$SEED template. The steps include creating a PDB, opening it, creating tablespaces, adding users, and assigning privileges. This guide is useful for learners and DBAs practicing Oracle Multitenant architecture
Table of Contents

CREATE PLUGGABLE DATABASE 
```sql
SQLCREATE PLUGGABLE DATABASE IS_PDB_27744
ADMIN USER mypdb_admin IDENTIFIED BY eric123
FILE_NAME_CONVERT = ('D:\ORACLE\ORADATA\ORCL\PDBSEED\', 'D:\ORACLE\ORADATA\ORCL\IS_PDB_27744\');
```
![Conceptual Diagram](https://github.com/erickishimwe/ISHIMWE-ERIC_ASSIGNMENT_2_27744/blob/fb432203eabe7ba65164766a76ec96b0e02b71d8/1.png) 

![Conceptual Diagram](https://github.com/erickishimwe/ISHIMWE-ERIC_ASSIGNMENT_2_27744/blob/f363b28fc4c347a031d6f3b665a7cfaca08c6a39/2.png) 

![Conceptual Diagram](https://github.com/erickishimwe/ISHIMWE-ERIC_ASSIGNMENT_2_27744/blob/f363b28fc4c347a031d6f3b665a7cfaca08c6a39/3.png) 

![Conceptual Diagram](https://github.com/erickishimwe/ISHIMWE-ERIC_ASSIGNMENT_2_27744/blob/f363b28fc4c347a031d6f3b665a7cfaca08c6a39/4.png) 






# Question 2: Create and Delete Pluggable Database (PDB)

Description:
This example demonstrates how to create a Pluggable Database (PDB) in Oracle and then delete it safely. The steps include:

Creating a new PDB from the PDB$SEED template.

Opening the new PDB.

Creating an administrative user for the PDB.

Deleting the PDB and its associated data files.

This exercise is useful for practicing PDB lifecycle management in Oracle Multitenant architecture.

```SQL
 CREATE PLUGGABLE DATABASE ISH_TO_DELETE_PDB_27744  ADMIN USER mypdb_admin IDENTIFIED BY  eric123  FILE_NAME_CONVERT = ('D:\ORACLE\ORADATA\ORCL\PDBSEED\', 'D:\ORACLE\ORADATA\ORCL\ISH_TO_DELETE_PDB_27744\');
```

![Conceptual Diagram](https://github.com/erickishimwe/ISHIMWE-ERIC_ASSIGNMENT_2_27744/blob/b1bea675849ad476221f69f3e33df45d12de69d7/2.1.png) 
![Conceptual Diagram](https://github.com/erickishimwe/ISHIMWE-ERIC_ASSIGNMENT_2_27744/blob/b1bea675849ad476221f69f3e33df45d12de69d7/2.2.png) 
![Conceptual Diagram](https://github.com/erickishimwe/ISHIMWE-ERIC_ASSIGNMENT_2_27744/blob/b1bea675849ad476221f69f3e33df45d12de69d7/2.3.png) 

```SQL
ALTER PLUGGABLE DATABASE ISH_TO_DELETE_PDB_27744 CLOSE IMMEDIATE;
```
![Conceptual Diagram](https://github.com/erickishimwe/ISHIMWE-ERIC_ASSIGNMENT_2_27744/blob/b1bea675849ad476221f69f3e33df45d12de69d7/2.5.png) 

