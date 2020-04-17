# Book Club Repository

Download the Oracle 19.3 EE For Linux ZIP and place into the 19.3.0 folder. The repo ignores it so that it is not committed since it is a large file.
http://www.oracle.com/technetwork/database/enterprise-edition/downloads/index.html

Ensure you have Docker installed: https://www.docker.com/products/docker-desktop

To build the docker image run this command in your terminal of choice. This command was tested as working in Windows Powershell but should work for Unix terminals as well.

docker build --build-arg DB_EDITION=ee -t oracle/database:19.3.0-${EDITION} .
