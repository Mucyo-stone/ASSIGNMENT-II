## Database Development with PL/SQL (INSY 8311)

## Instructor: Eric MANIRAGUHA
## Student Name: Mucyo Stone
## Student ID: 29084

## 📌 PROJECT OVERVIEW

This project demonstrates the management of Oracle Multitenant Architecture using Oracle Database 21c Express Edition.

## The main objective was to practice:

Creating Pluggable Databases (PDBs)

Opening and verifying PDB status

Creating and managing users inside PDBs

Closing and deleting PDBs

Monitoring database activities using Oracle Enterprise Manager (OEM)

This project strengthened my understanding of container databases (CDB) and pluggable databases (PDB) in Oracle.

## 💻 MY ENVIRONMENT

Database: Oracle Database 21c Express Edition

Operating System: Windows 11 Pro (64-bit)

## Tools Used:

## SQL*Plus

## Oracle Enterprise Manager (OEM)

##  TECHNICAL TASKS
## ✅ Task 1: Creating My Permanent PDB

I created a permanent Pluggable Database named:

ms_pdb_29084


Inside this PDB, I created a user:

mucyo_plsqlauca_29084


To create the PDB, I used the FILE_NAME_CONVERT clause to copy data files from the seed database (PDB$SEED).

## After creating the PDB:

I opened it using ALTER PLUGGABLE DATABASE OPEN;

Verified its status using SHOW PDBS;

Confirmed it was ready for future class practical work

## 📌 Result: PDB successfully created and opened.

##  Task 2: PDB Lifecycle Management (Create and Delete)

To demonstrate lifecycle management, I created a temporary PDB named:

ms_to_delete_pdb_29084


Steps performed:

Created the temporary PDB

Verified its existence

Closed the PDB

Dropped it using:

DROP PLUGGABLE DATABASE ms_to_delete_pdb_29084 INCLUDING DATAFILES;


The INCLUDING DATAFILES option ensured complete removal of associated files from storage.

## Result: Temporary PDB successfully created and deleted.

## Task 3: Oracle Enterprise Manager (OEM)

I accessed the Oracle Enterprise Manager web interface.

From the dashboard, I:

Verified that the Oracle database instance was running

Confirmed the created PDB was visible

Observed system health and performance indicators

## Result: OEM reflected all completed PDB tasks correctly.

## Challenges Faced
## 1️⃣ Password Errors

I experienced login errors because my password contained special characters such as @.

## ✅ Solution:
I enclosed the password inside double quotes when connecting in SQL*Plus.

Example:

CONNECT stone ..../ stone#12000

## 2️⃣ OEM Login Issues

Initially, I could not access the OEM dashboard.

## ✅ Solution:

Switched to a compatible web browser

Used the correct administrative login format

Ensured Oracle services were running

## Professional & Ethical Note

## “Excellence is never an accident; it is the result of discipline, commitment, and integrity.”
As future database professionals, we understand that precision, discipline, and integrity are non-negotiable.
##  This project reflects my commitment to upholding professional and ethical standards in all database work.
