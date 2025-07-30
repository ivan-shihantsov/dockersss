## WordPress + MySQL

### try 1: only mysql + wordpress

```
cd 1
docker compose up -d
```
and open wordpress localhost:8080<br>


### try 2: mysql + wordpress + phpmyadmin + new network

```
cd 2
docker compose up -d
```

and open wordpress on localhost:8080<br>
then open phpmyadmin on localhost:8081<br>
* mysql user: user1
* mysql pass: pass123


### try 3: mysql + wordpress + phpmyadmin + new network + secrets

```
cd 3
docker compose up -d
```

As in the previous example, both wordpress and phpmyadmin can be opened in browser<br>


