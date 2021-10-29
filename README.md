# Docker-Postgres
Want a postgres db up and running in a second, this yaml file is your guy. 


## Test it out
If you have psql installed,
psql -h 127.0.0.1 -p 5432 -U postgres postgres



## Start up
```
docker-compose up -d
```

## End it

```
docker-compose down --volumes
```

## Get a weird address already in use error?
I got you
```
sudo lsof -i -P -n | grep 5432  

```
after you find postgres container
```
sudo kill "pid"
```
