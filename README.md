# dbli
Sometimes you just need to run a query to a database. This intends to remove most of the boilerplate for that. No need to setup ORM or models, just input the connection data and type your query. You need something more complex? Then this won't get in the way, you can retrieve a connection a manage the transaction manually.

## Installation

```
pip install thisIsStillNotDeployedInPip
```

## Query example
```
from dbli import database

db = database((user, host, password, port))
print(db.ask(select * from yourtable t where t.id = :1, [15]))
```

## Transaction example
```

```
 
# DBs supported

## Postgree
Depends on psycopg2
