# Ontotext GraphDB set-up process

Pre-configured Docker Images of tools/libraries/language(s): Python 3 + Java 8 + Maven 3.5 and GraphDB 10.x


## You need to get your own free download version for docker to build successfully
- Default Docker build-arg is set to use 10.0.2 version. You can change that in "docker.env" file.
```
GRAPHDB_VERSION=10.0.2
```
- You can go to Ontotext web site to register to download the free version, **graphdb-free-10.0.2-dist.zip**, and place in this directory as shown below.
- Then, you can use (build.sh: optional to build your own locally) run scripts to start using.
- Optional - Adding the Licenses is depends on individual email registrations. Ontotext-Grapdb support will share individual or group licenses via support email.
- NOTE: used existing docker repo "openkbs"
```
.
├── build.sh
├── commit-push.sh
├── docker-compose.yml
├── docker.env
├── Dockerfile
├── graphdb-free-<GRAPHDB_VERSION>-dist.zip or graphdb-ee-<GRAPHDB_VERSION>-dist.zip
├── Makefile (not recommended to use this)
├── README.md
└── run.sh

```

# Build (if you want to build your own image)
```
./build.sh
```

# Run
```
./run.sh
```

By default, you can access GraphDB Workbench Web UI at


* http://<ip_address>:27200/
* [http://0.0.0.0:27200/](http://0.0.0.0:27200/) 
* [http://127.0.0.1:27200/] (http://127.0.0.1:27200/) 
* [http://localhost:27200/] (http://localhost:27200/)
