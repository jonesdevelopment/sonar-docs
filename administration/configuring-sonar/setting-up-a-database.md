# Setting up a database

There are currently two types of databases which are supported by Sonar: [MySQL](https://www.mysql.com/) and [MariaDB](https://mariadb.org/)

```yaml
type: NONE # No database selected, Sonar will cache all users in memory
```

```yaml
type: MYSQL # MySQL selected
```

```yaml
type: MARIADB # MariaDB selected
```



The host and port for the database is where Sonar will connect when trying to access the database.

```yaml
host: localhost # Use localhost to connect to the database
```

```yaml
port: 3306 # Default SQL port
```



The name of the SQL database can be modified to your liking. It represents the database Sonar will use to store all the verified players. Please choose an appropriate name or leave this as the default.

```yaml
name: sonar
```



The username and password are used by Sonar to authenticate the connection to the database. The connection will fail if no username or password are given.

```yaml
username: 'my_username'
```

```yaml
password: 'my_p@ssw0rd!'
```

\
The last setting describes how many days Sonar should keep verified players in the database. This option is important as it keeps the database clean since it always removes outdated entries.

```yaml
maximum-age: 5
```

> Note: This value represents the time in days
