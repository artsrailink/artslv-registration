# Registration Service (Note Reg service akan jarang berubah)

# Asumsinya registration service always run di ip 172.16.9.45


How to run:

```sh

# Build

mvn clean package docker:build

# Masuk ke 172.16.9.45 dan pull dari registry

docker pull gitlab.kereta-api.co.id:5000/arts-registration

# run

docker run -p 8761:8761 --name reg-service gitlab.kereta-api.co.id:5000/arts-registration


```

Once all the services are up, the following URLs will be available
