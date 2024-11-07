ARG BUILD_FROM
FROM $BUILD_FROM

RUN \
  apk add --no-cache \
    python3 py3-pip
RUN \
    pip3 install https://github.com/NickWaterton/samsung-tv-ws-api/archive/master.zip[async,encrypted]
# Copy data for add-on
COPY run.sh /
COPY art.py /


RUN chmod a+x /run.sh

CMD [ "/run.sh" ]
