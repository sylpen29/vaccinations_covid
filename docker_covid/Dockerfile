FROM python
ENV DEBIAN_FRONTEND=noninteractive
RUN apt-get update \
    && pip --disable-pip-version-check --no-cache-dir install mysql-connector
ENV DEBIAN_FRONTEND=dialog