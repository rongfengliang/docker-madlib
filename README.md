# Docker Madlib

> Dockerized madlib (made easy) using postgres 10.

1) Open a terminal and run `docker-compose up` inside this folder.
2) Open another bash terminal and run `docker-compose exec db bash`
3) Run `/usr/local/madlib/bin/madpack -p postgres -c postgres/root@localhost:5432/sample install`
4) Run install check on all modules `/usr/local/madlib/bin/madpack -p postgres -c postgres/root@localhost:5432/sample install-check`
5) Now you can exit from the last bash terminal, run `exit`
6) Navigate to `http://127.0.0.1:8080` and login with adminer using the following credentials:
   - **System**: PostgresSQL
   - **Server**: db
   - **Username**: postgres
   - **Password**: root
   - **Database**: sample
7) Go to "madlib" schema and check the install.

8)  hasura/graphql-engine address 
    - http://localhost:9090

**Notes:**
 - If you want to access through Navicat or similar software, just replace the "db" server host by 127.0.0.1 or localhost 
 

