# redmine
Redmine for MSSQL (Microsoft SQL-Server) running on Docker
This project is about running redmine on Docker using a Linux-Version of Microsoft SQL-Server Express 2019 (this "only" needs 2 GB RAM).

The concept:
- it must be secure, robust and lightweight - that's why I am using Alpine-Linux https://alpinelinux.org/ (Alpine takes only 5 MB!!!)
- using a CMS-Plugin redmine is pre-configured to act like a real website
