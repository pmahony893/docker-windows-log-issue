FROM openjdk:8-jre@sha256:e2d69dc0ee0a49d04665cc9e4c9f0fafc25ffb246821f840136efec6a1bcb998
RUN apt update && apt install -y bash
WORKDIR /app
COPY run.sh /app
CMD ["bash", "run.sh"]