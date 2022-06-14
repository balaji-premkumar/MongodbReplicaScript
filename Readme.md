
# Mongodb Replicaset Scripts

Mongodb Replication using 2 nodes using mongodb.

In this application i have used the percona mongodb 4.4 version for enterprise grade mongodb service




## Installation

Running this scripts, you guys need to have the docker in your pc or mac.

```bash
  git clone https://github.com/balaji00710/MongodbReplicaScript.git
  cd MongodbReplicaScript
```

Once entered into the directory of cloned files then run this command
```bash
  docker-compose up -d
```

wait till the containers up and running. once containers are up and running
```bash
docker exec -it mongo1 bash
```

run this script to activate the replicaset config
```bash
/scripts/rs-init.sh
```

now the mongodb is configured as replicaset. you guys can access the database using this given mongodb url
```bash
mongodb:localhost:27021,localhost:27022,localhost:27023/?replicaSet=dbrs&readPreference=primaryPreferred
```
    