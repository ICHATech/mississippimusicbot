FROM alpine:3.4
RUN apk update \
 && apk add python3-dev ca-certificates gcc make linux-headers musl-dev ffmpeg libffi-dev
ADD . /usr/src/MusicBot
WORKDIR /usr/src/MusicBot
VOLUME /usr/src/MusicBot/config
RUN pip3 install -r requirements.txt

CMD python3.5 run.py
