# dbs-docker-compose
Template for build database image with docker-compose for dev purpose :rocket:

### How to start ?

Move into kind db need to use

For instance:
```bash
# For example we need to uses mysql db
$ cd mysql
```
<hr />
<p>And now, we use `Make` to start 🚀 </p>

```bash
# Wake up container
$ make up

# Run and build without detach mode
$ make build

# Run and build with detach mode
$ make upd

# Down container and persist volume
$ make down

# Down container and remove persist volume
$ make downvl

```
