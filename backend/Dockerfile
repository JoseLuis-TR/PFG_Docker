FROM openjdk:11-jdk-slim
COPY . /app
COPY wait-for-it.sh /app/wait-for-it.sh
WORKDIR /app
RUN chmod +x mvnw
RUN ./mvnw clean install
EXPOSE 8080
CMD ["java", "-jar", "target/PFG_haven-0.0.1-SNAPSHOT.jar"]