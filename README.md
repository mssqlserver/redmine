Redmine image for Docker (Alpha version - in progress)
========================
This project is about running a ready to use redmine on Docker using a Linux-Version of Microsoft SQL-Server Express 2019. The goal is keep this project up to date so that always the latest version of redmine will be supported.

The concept:
- be secure, robust and lightweight - using Alpine-Linux https://alpinelinux.org/ (Alpine takes only 5 MB!!!)
- using a CMS-Plugin redmine is pre-configured to act like a real website
- Microsoft SQL-Server Express 2019 running on linux (this version "only" needs 2 GB RAM)
- CMS-Plugin redmine is pre-configured to act like a real website
- accessing the redmine-database using tools like "Microsoft SQL Server Management Studio"
- the project contains a step-by-step-guide which lets novice docker-users run redmine on docker
- documentation of how to install redmine plugins & themes you have purchased or downloaded 

More information:
https://hub.docker.com/r/mssqlserver/redmine

Redmine image for Docker with several extensions and improvements.

This Redmine image is based on the [official -/redmine image][1] plus a
RAILS_RELATIVE_URL_ROOT patch, support for additional SSL certificates
and a pre-installed git-remote plugin.

RAILS_RELATIVE_URL_ROOT patch
-----------------------------

Supports shifting the complete Redmine instance into a subdirectory by
defining an environment variable
`RAILS_RELATIVE_URL_ROOT=/sub/url/to/redmine`. If the variable is
missing, Redmine is served from the base URL.

Additional SSL certificates
---------------------------

Any certificates present in the `/usr/local/share/ca-certificates/`
directory are added to the list of CAs trusted by OpenSSL on start of
the container.

git-remote plugin
-----------------

Comes with the [git-remote][2] plugin pre-installed.

[1]: https://hub.docker.com/_/redmine
[2]: https://github.com/dergachev/redmine_git_remote
