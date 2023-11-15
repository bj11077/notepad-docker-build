FROM openjdk:17
RUN mkdir -p /data
RUN mkdir -p /applications

ENV SAVE_DIR "/data"
ENV WORK_DIR "/applications"

COPY . /applications
WORKDIR /applications
ENTRYPOINT ["java","-jar","/applications/notepad-0.0.1-SNAPSHOT.jar","--spring.config.location=/applications/application.yml"]
