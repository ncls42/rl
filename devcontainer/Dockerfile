# Utilise Ubuntu 22.04 (comme à l'école)
FROM ubuntu:22.04

# Empêche les prompts interactifs
ENV DEBIAN_FRONTEND=noninteractive

# Mise à jour + outils de base
RUN apt update && apt install -y \
    build-essential \
    git \
    curl \
    lsb-release \
    cmake \
    gdb \
    make \
    python3 \
    python3-pip \
    python3-venv \
    software-properties-common \
    pkg-config \
    unzip \
    bash \
    && apt clean

# Configure Python pour éviter les warnings
RUN ln -s /usr/bin/python3 /usr/bin/python

# Ajoute un utilisateur non-root si besoin (optionnel)
