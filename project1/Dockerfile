FROM java:8

RUN mkdir /app
#COPY ./build/libs/project1.jar /app/app.jar
COPY ./src /app/
RUN cd /app & gradle build

CMD ["java", "-jar", "/app/app.jar"]
