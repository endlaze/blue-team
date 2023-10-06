# Ubuntu x86-64 container

# Build: docker build --platform linux/amd64 -t <IMAGE_NAME> <PATH>
# Exec:  docker run -td --platform linux/amd64 <IMAGE_NAME>

# --- Pull Ubuntu x86-64 image ---
FROM amd64/ubuntu

# --- Update packages & Install locales, wget and curl ----

RUN apt update && apt upgrade -y
RUN apt install -y \
    locales \
    wget \
    curl

# ---- Set en_US.UTF-8 encoding settings ----

RUN locale-gen en_US.UTF-8
ENV LANG en_US.UTF-8
ENV LANGUAGE en_US:en
ENV LC_ALL en_US.UTF-8
