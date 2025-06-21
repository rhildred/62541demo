FROM mcr.microsoft.com/devcontainers/universal:latest

RUN curl --output /usr/share/keyrings/nginx-keyring.gpg  \
      https://unit.nginx.org/keys/nginx-keyring.gpg

RUN echo "deb [signed-by=/usr/share/keyrings/nginx-keyring.gpg] https://packages.nginx.org/unit/debian/ bookworm unit\ndeb-src [signed-by=/usr/share/keyrings/nginx-keyring.gpg] https://packages.nginx.org/unit/debian/ bookworm unit" > /etc/apt/sources.list.d/unit.list

RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
    && apt-get -y install git build-essential gcc pkg-config cmake python3 cmake-curses-gui libmbedtls-dev check libsubunit-dev libpcap-dev python3-sphinx graphviz python3-sphinx-rtd-theme libavahi-client-dev libavahi-common-dev unit unit-dev unit-php unit-python3.12 ansible
