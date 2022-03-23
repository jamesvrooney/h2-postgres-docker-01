
### Using docker for Postgres DB and PgAdmin (for local testing)
#### Start running both containers
```
docker compose up -d
```

#### Access PgAdmin via the browser
[PgAdmin - running on docker](http://localhost:5050/browser/)

##### Initial setup (values for Host, Username & Password must match what we have in the docker-compose file)
* Set Master Password for pgAdmin - password
* Name: james-test-server
* Host: postgres
* Username: jamesvrooney
* Password: password

##### When creating the database the name we use must be used in application.yml file
The database was called **dogs** when created.
```
url: jdbc:postgresql://localhost:5432/dogs
```


