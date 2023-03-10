FROM mambaorg/micromamba
WORKDIR /content/
COPY env.yml /home/mambauser/env.yml
RUN micromamba install -y -n base -f /home/mambauser/env.yml
USER root
RUN apt update && apt install xorg libsqlite3-0 aria2 -y
