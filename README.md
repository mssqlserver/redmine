# Redmine out of the box using MSSQL (both on Linux)
pre-configured redmine on a lightweight linux using MSSQL Express 2019 for linux

This project is about running redmine on Docker using a Linux-Version of Microsoft SQL-Server Express 2019

The concept:
- Microsoft SQL-Server 2019 running on linux (this version "only" needs 2 GB RAM)
- secure, robust and lightweight - using Alpine-Linux https://alpinelinux.org/ (Alpine takes only 5 MB!!!)
- CMS-Plugin redmine is pre-configured to act like a real website
- accessing the database using tools like "Microsoft SQL Server Management Studio"

More information:
https://hub.docker.com/r/mssqlserver/redmine

This project has started in October 2019
Based on https://hub.docker.com/r/menlosystems/redmine/
