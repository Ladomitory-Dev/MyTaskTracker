FROM openjdk:25-rc-jdk

ARG appName=tasktracker
ARG appVersion=0.0.1

RUN ["mkdir", "./jar"]

COPY ./target/${appName}-${appVersion}.jar ./jar

EXPOSE 8080

CMD ["java", "-jar", "./jar/tasktracker-0.0.1.jar"]
#Build (in dir "./tasktracker"): docker build -t ladomitorydev/tasktracker:0.0.1 --platform linux/amd64 --no-cache ./
#Build (in main dir): docker build -t ladomitorydev/tasktracker:0.0.1 --platform linux/amd64 --no-cache ./tasktracker