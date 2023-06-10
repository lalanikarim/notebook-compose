Jupyter Lab Container Compose
=============================

Run [Jupyter Lab Notebooks](https://jupyter.org/) locally using containers.

Why run Jupyter Lab locally?
----------------------------

A few reasons to run Jupyter Lab locally include, but are not limited to:

* Learn [python](https://www.python.org/)
* Build and test AI/ML models locally
* A free alternate to [Google Colab](https://colab.research.google.com/) and you keep all your files

Why use containers?
---------------------

While you can install and run Jupyter Lab locally on your computer by following simple instructions from [https://jupyter.org/install], your mileage will likely vary. The main issue you can potentially run into will be around your version of locally installed Python, and how updating Python or your OS may break any underlying dependencies. This will result in a disjointed and unreliable experience.

Containers provide you with sandboxes that are unaffected by the host OS. Running Jupyter Lab within a container will mean that it will run predictably every time, unaffected by the changes to the host OS or any other system updates. It will also allow you to replicate your setup on any other computer where the container runtime is available.

Prerequisites
--------------

You'll need to have a compatible container runtime like [Docker](https://www.docker.com/) or [Podman](https://podman.io/).  
You'll also need the ability to run container compose specs like [docker compose](https://docs.docker.com/compose/install/) or [podman compose](https://docs.docker.com/compose/install/).  

Note that additional prerequisites may be needed in order to install your preferred container runtime and the compose executor.  
Additionally, you may also need to install [git-scm](https://git-scm.com/) if you want to download the files using `git clone`.

Launching Jupyter Lab
---------------------

1. Clone the repo or download the archive
You may download the files as zip file from here <https://github.com/lalanikarim/notebook-compose/archive/refs/heads/main.zip> and extract files in a folder.  

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

3. Open Jupyter Lab in your browser by visiting <http://localhost:8888>
