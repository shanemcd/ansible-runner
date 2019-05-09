FROM fedora:29

RUN dnf install -y make mock python-pip which git

# Fix output of rpm --eval '%{?dist}'
# RUN sed -i "s/.el7.centos/.el7/g" /etc/rpm/macros.dist

# Newer version of setuptools needed for pipenv
RUN pip install -IU pip setuptools
RUN pip install -IU pipenv ansible

