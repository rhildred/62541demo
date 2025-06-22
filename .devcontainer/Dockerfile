FROM mcr.microsoft.com/devcontainers/universal:latest

RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
    && apt-get -y install git build-essential gcc pkg-config cmake python3 cmake-curses-gui libmbedtls-dev check libsubunit-dev libpcap-dev python3-sphinx graphviz python3-sphinx-rtd-theme libavahi-client-dev libavahi-common-dev ansible
