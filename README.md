# oracle_pdb_ass_II_-28886-_-Kelly-
# Oracle Pluggable Database Assignment II – Documentation
# 1. Overview of Tasks

This assignment focused on practical implementation of Oracle Multitenant Architecture using Pluggable Databases (PDBs). The objective was to demonstrate the ability to create, manage, verify, and delete PDBs within a Container Database (CDB) environment.

The assignment consisted of three major technical tasks:

1.Creating a new Pluggable Database using a strict naming convention.
<img width="1041" height="505" alt="pluggable created successfully" src="https://github.com/user-attachments/assets/209a966a-7e62-45df-b462-9a063583cd57" />


2.Creating a database user inside the PDB for future coursework.
<img width="524" height="232" alt="USER CREATED" src="https://github.com/user-attachments/assets/b25893e9-6a14-41e0-8c35-432e2c2d0617" />

I also Granted a USER
<img width="809" height="385" alt="user created and granted sucessfully" src="https://github.com/user-attachments/assets/2f0b048e-047f-487f-a7d8-7d663208e8d6" />
3.Creating and completely deleting a temporary PDB.
Creation of a temporary PDB.
<img width="865" height="403" alt="pluggable to delete created sucessfully" src="https://github.com/user-attachments/assets/53355f1d-9e49-4489-8960-6800477bdbf4" />
Deletation of a temporary PDB.
<img width="758" height="286" alt="Pluggable drop_deleted successfully" src="https://github.com/user-attachments/assets/5c0cf07c-c3e0-4ead-962c-346f0b08685b" />

4.Configuring and accessing Oracle Enterprise Manager (OEM) to verify the database environment visually.

Each task required proper verification through commands and screenshots to confirm successful execution.


2. Oracle Environment Used

# The assignment was completed using the following environment:

* Database System: Oracle Database 21c

* Architecture: Multitenant Architecture (CDB and PDB)

* Database Tool: SQL Developer

* Management Interface: Oracle Enterprise Manager

Operating System: [Specify: Windows]

Oracle Multitenant Architecture allows multiple pluggable databases (PDBs) to exist inside one container database (CDB). This architecture improves resource management, scalability, and administrative efficiency.

SQL Developer was used to execute all administrative commands such as creating PDBs, opening databases, creating users, granting privileges, and dropping databases.

Oracle Enterprise Manager (OEM) was used to visually confirm database configuration and monitor the system environment.

# Task 1 – Creation of a New Pluggable Database

The first task required creating a new PDB following an exact naming convention. The database was created from the seed database and assigned an administrative user.

After creating the PDB, it was opened in READ WRITE mode to allow user operations. The session container was switched to the newly created PDB, and a dedicated user account was created inside it. Required privileges such as CONNECT and RESOURCE were granted to ensure the user could perform future database activities.

Verification was done using:

SHOW PDBS to confirm the open status.

Querying DBA_USERS to confirm the user creation.

This task demonstrated proper PDB creation, configuration, and user management within a multitenant environment.

# Task 2 – Creation and Deletion of a Temporary PDB

The second task involved creating a temporary PDB and then deleting it completely.

First, the temporary PDB was created using the required naming convention. Its existence was verified using container listing commands. The PDB was then closed to ensure it was not in use.

The database was permanently removed using the DROP PLUGGABLE DATABASE command with the INCLUDING DATAFILES clause to ensure that all associated data files were deleted from the system.

A final verification confirmed that the temporary PDB no longer appeared in the container list.

This task demonstrated safe database removal procedures and proper cleanup of database resources.

# Task 3 – Oracle Enterprise Manager (OEM)

The third task required configuring and accessing Oracle Enterprise Manager.

OEM was started and accessed through a web browser interface. After logging in with administrative privileges, the dashboard displayed:

Database status

Container database information

Created pluggable databases

System performance overview

The dashboard confirmed that the created PDB was active and properly configured. This task demonstrated the ability to monitor and manage Oracle databases using graphical tools in addition to command-line utilities.

# 4. Challenges Faced and Solutions

During the completion of the assignment, several minor technical challenges were encountered:

1. PDB Not Opening Automatically

After creation, the PDB was initially in MOUNTED mode.
Solution: Used the ALTER PLUGGABLE DATABASE OPEN command to open it in READ WRITE mode.

2. Listener or Connection Issues

There were temporary connection issues when accessing the database services.
Solution: Restarted the listener service using the lsnrctl start command and verified service status.

3. OEM Access Issues

At first, the OEM dashboard did not load due to port configuration.
Solution: Verified that the OEM service was running and ensured the correct port (5500) was accessible through the firewall.

All issues were resolved successfully through troubleshooting and command verification.

# 5. Integrity Statement

I hereby confirm that this assignment was completed independently in my own Oracle environment. All commands were executed individually, and all screenshots reflect my original work. I have followed academic integrity guidelines and have not copied or misrepresented any part of this assignment.



# FINAL CHECK LIST
1.Correct PDB names used :CHEKED
2.User created inside the PDB: CHEKED
3.Temporary PDB created and deleted :CHEKED
OEM dashboard screenshot included :CHECKED
GitHub repository is PUBLIC :CHEKED
README is clear and professional: CHEKED
Deadline respected : YES

