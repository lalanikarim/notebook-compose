Jupyter Lab Container Compose
=============================

Run [Jupyter Lab Notebooks](https://jupyter.org/) locally using containers.

Why run Jupyter Lab locally?
----------------------------

* Learn [python]()

Why using containers?
---------------------

Prerequisites
--------------

You'll need to have a compatible container runtime like [Docker](https://www.docker.com/) or [Podman](https://podman.io/).  
You'll also need the ability to run container compose specs like [docker compose](https://docs.docker.com/compose/install/) or [podman compose](https://docs.docker.com/compose/install/).  

Note that additional prerequisites may be needed in order to install your preferred container runtime and the compose executor.  
Additionally, you may also need to install [git-scm](https://git-scm.com/) if you want to download the files using `git clone`.

Launching Jupyter Lab
---------------------

1. Clone the repo or download the archive
You may download the files as zip file from here [https://github.com/lalanikarim/notebook-compose/archive/refs/heads/main.zip] and extract files in a folder.  

Alternatively, may clone the repo using the following command
```
git clone git@github.com:lalanikarim/notebook-compose.git
```

Once you the files extracted or cloned, using your terminal, `cd` into the folder.

```
cd notebook-compose
```

2. Launch the container

```
docker compose up
```
Or
```
podman-compose up
```

3. Open Jupyter Lab in your browser by visiting [http://localhost:8888]
