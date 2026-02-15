**Oracle Pluggable Database Assignment II**

**Course:** Database Development with PL/SQL (INSY 8311)

**Student Name:** Fiston

**Student ID:** 28330

## OVERVIEW

> In this assignment, I worked on implementing Oracle Multitenant Architecture using Oracle Database 21c Express Edition.
> 

> My goal was to create and manage Pluggable Databases (PDBs), create users inside a PDB, delete a PDB, and use Oracle Enterprise Manager (OEM) to monitor and manage the database.
> 

## **Oracle Environment Used**

> Oracle Database 21c Express
> 

> Platform: Microsoft Windows
> 

> SQL Plus
> 

> Oracle Enterprise Manager (OEM)
> 

## **Task 1: Create a New Pluggable Database**

### **PDB Created:**

<aside>
💡

FI_PDB_28330

</aside>

### Steps performed:

1. Connected to SQL Plus as SYSDBA.
2. Created the pluggable database using the required naming convention.
3. Opened the PDB.
4. Switched session to the new PDB.
5. Created the user:

> fiston_plsqlauca_28330
> 

<aside>
💡

1. Granted necessary privileges to the user.
</aside>

> The PDB was successfully created and opened in READ WRITE mode.
> 

> The user was created inside the PDB and will be used for future PL/SQL work.
> 

## **Task 2: Create and Delete a Temporary PDB**

### **Temporary PDB Created:**

<aside>
💡

FI_TO_DELETE_PDB_28330

</aside>

### Steps performed:

1. Switched to CDB$ROOT.
2. Created the temporary PDB.
3. Verified its existence using SHOW PDBS.
4. Dropped the PDB using INCLUDING DATAFILES.
5. Confirmed it no longer existed.

> The temporary PDB was successfully created and completely removed from the system.
> 

## **Task 3: Oracle Enterprise Manager (OEM)**

<aside>
💡

I accessed Oracle Enterprise Manager Database Express through the browser.

</aside>

### The dashboard confirmed:

- Oracle environment running properly
- FI_PDB_28330 visible
- Database performance and storage statistics displayed
- My environment successfully configured

> Screenshot of the OEM dashboard is included in the screenshots folder.
> 

### **Challenges Faced**

<aside>
💡

During the assignment, I encountered a few errors:

</aside>

- ORA-00922 when running multiple SQL statements on one line
- ORA-65040 when attempting to create a PDB while connected to another PDB instead of CDB$ROOT

### These issues were resolved by:

- Executing commands separately
- Switching correctly to CDB$ROOT before creating a new PDB

<aside>
💡

These challenges helped me better understand Oracle Multitenant Architecture.

</aside>

## **Integrity Statement**

> “All sources were properly cited. Implementations and analysis represent original work. No AI
generated content was copied without attribution or adaptation.”
>
