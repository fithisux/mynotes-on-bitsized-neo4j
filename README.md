# Welcome to my Neo4J bit-sized notes!

These are my notes while "running" the excellent bit-sized neo4j tutorials [here](https://www.youtube.com/watch?v=Niys6g6NFfw&list=PL9Hl4pk2FsvVShoT5EysHcrs-hyCsXaWC). There are 3 kinds of notebooks and a docker-compose file that act as a "code transcript" or reference. I attempt to make the notebooks self contained.
The first called __for-sandbox.ipynb__ is used against the GDS sandbox that you can create according to the instructions of lesson 1. These have the Cypher or APOC snippets presented during the lesson as python strings to be executed through the neo4j driver. These are run against the "Game of Thrones" dataset.
The second called __for-local.ipynb__ is used against an empty instance of Neo4J that is initiated through the __docker-compose.yml__ file included in the repo which is the convenient [Official Neo4J image](https://hub.docker.com/_/neo4j). This has the snippets used in the lessons against an empty database. After running you dockerized neo4j. The third notebook is __icij-sandbox.ipynb__ which holds the code for FastRP on the Paradise papers dataset.

```
docker-compose up -d
```

connect to

```
http://localhost:7474/browser/
```
with the defaults neo4j/neo4j credentials. Now you can setup a pasword that will be used by your jupyter lab notebook.

The code has been tested with Python 3.10.3 and covers up to and including lesson 18 about Fast Random Projections. Lesson 18 has in the [bit-sized repo](https://github.com/cj2001/bite_sized_data_science) a dedicated notbook that can be used with the docker-compose.yml provided here But this one does not work with GDS2.0. So I provide a modified one.
A __requirements.txt__ is included.

>> It is advised to create a virtualenv through
>```
>python -m venv myvenv && source myvenv/bin/activate
> pip install -r requirements.txt
>```

Enjoy!
