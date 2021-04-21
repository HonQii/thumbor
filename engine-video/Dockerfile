ARG THUMBOR_TAG=latest
FROM minimalcompact/thumbor:$THUMBOR_TAG

LABEL maintainer="honqii"

COPY requirements.txt /app/requirements.txt
RUN pip install --trusted-host None --no-cache-dir \
    -r /app/requirements.txt

COPY conf/thumbor.conf.tpl /app/thumbor.conf.tpl

