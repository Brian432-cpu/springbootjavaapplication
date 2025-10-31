# ====== Build stage ======
FROM eclipse-temurin:21-jdk-jammy AS builder

WORKDIR /opt/app
COPY .mvn/ .mvn
COPY mvnw pom.xml ./
RUN ./mvnw dependency:go-offline
COPY ./src ./src
RUN ./mvnw clean package -DskipTests

# ====== Runtime stage (Distroless) ======
FROM gcr.io/distroless/java17-debian12

WORKDIR /opt/app
COPY --from=builder /opt/app/target/*.jar app.jar

EXPOSE 8080
ENTRYPOINT ["java", "-jar", "/opt/app/app.jar"]
