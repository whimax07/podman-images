FROM docker.io/library/fedora:latest

RUN dnf install -y git-all
RUN dnf install -y which

RUN dnf install -y dbus-x11
RUN dnf install -y gedit

WORKDIR /home/dev

COPY --chmod=777 configure /home/dev
RUN /home/dev/configure
