# trans-server-https-portal-docker-compose

[Trans server](https://github.com/nwtgck/trans-server-akka) on HTTPS powered by [https-portal](https://github.com/SteveLTN/https-portal)

## Run the server

### Step 1

Modify domain in [docker-compose.yml](docker-compose.yml) (Replace "trans-akka.ml" with your domain). 

### Step 2

Run docker-compose like the following.

```bash
cd <this repo>
docker-compose up
```

Wait for long time when you see the following message.

```
...
https-portal_1  | This is going to take a long time
...
````

Done!

## Data persistence

All data for persistence are under `./docker_volumes`.

* Trans DB - `./docker_volumes/trans-db`
* Certificates - `./docker_volumes/ssl_certs`.
