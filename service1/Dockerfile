FROM alpine:latest
WORKDIR /service1
RUN apk update && apk add bash
COPY run.sh /service1
CMD ["bash", "run.sh"]