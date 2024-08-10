---
description: >-
  Sonar can be connected to a database to retain verified player data even after
  server restarts.
---

# Setting up a database

{% hint style="info" %}
IP addresses are stored in plain text, so ensure your database is secure.
{% endhint %}

Defines the type of database used by Sonar. Options include `NONE`, `MYSQL`, `MARIADB`, and `H2`. Default: `NONE`

```yaml
type: NONE
```

Specifies the file name for the `H2` database stored in Sonar's plugin directory. Default: `verified_players`

```yaml
filename: verified_players
```

The host address for SQL database authentication. Default: `localhost`

```yaml
host: localhost
```

The port number for SQL database authentication. Default: `3306`

```yaml
port: 3306
```

The name of the SQL database. Default: `sonar`

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

The number of days Sonar should retain verified players in the database. Default: `5`

```yaml
maximum-age: 5
```
