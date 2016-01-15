FROM java:8

RUN mkdir /app
#COPY ./build/libs/project1.jar /app/app.jar
COPY ./ /app/
RUN cd /app && ./gradlew build

CMD ["java", "-jar", "/app/build/libs/project1.jar"]
