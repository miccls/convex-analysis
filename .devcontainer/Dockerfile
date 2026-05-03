FROM debian:stable-slim

ARG DEBIAN_FRONTEND=noninteractive

# Basic setup and locale.
RUN <<EOF
set -eux

apt-get update
apt-get install -y --no-install-recommends \
  ca-certificates \
  locales

echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen
locale-gen
EOF

ENV LANG=en_US.UTF-8 \
    LANGUAGE=en_US \
    LC_ALL=en_US.UTF-8 \
    LC_CTYPE=en_US.UTF-8

# Install stuff we need for development, LaTeX compilers etc
RUN <<EOF
set -eux

apt-get update
apt-get install -y --no-install-recommends \
    sudo \
    git \
    texlive-latex-base \
    texlive-latex-recommended \
    texlive-latex-extra \
    texlive-fonts-extra \
    texlive-bibtex-extra \
    latexmk \
    biber \
    texlive-extra-utils \
    libyaml-tiny-perl \
    libfile-homedir-perl \
    libunicode-linebreak-perl

# Clean up apt cache
apt-get clean
rm -rf /var/lib/apt/lists/*
EOF

# https://code.visualstudio.com/remote/advancedcontainers/add-nonroot-user
ARG USERNAME=convex-analyzer
ARG USER_UID=1000
ARG USER_GID=$USER_UID

RUN groupadd --gid $USER_GID $USERNAME \
    && useradd --uid $USER_UID --gid $USER_GID -m $USERNAME \
    && echo $USERNAME ALL=\(root\) NOPASSWD:ALL > /etc/sudoers.d/$USERNAME \
    && chmod 0440 /etc/sudoers.d/$USERNAME

# [Optional] Set the default user. Omit if you want to keep the default as root.
USER $USERNAME

# Set a working directory inside the container.
WORKDIR /workspace
