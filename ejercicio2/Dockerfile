FROM maven:3.8.3-openjdk-17 as build

# Apartado i

# Apartado ii

RUN mvn install -DskipTests
# En la siguiente linea hay que completar algo para el Apartado iii
RUN mkdir -p target/dependency && (cd target/dependency;  -xf ../*.jar)



FROM openjdk:17-jdk-alpine
VOLUME /tmp


# Apartado iv

# En las 3 siguientes lineas, hay que incluir algo para completar el Apartado v
COPY --from=build /BOOT-INF/lib /app/lib
COPY --from=build /META-INF /app/META-INF
COPY --from=build /BOOT-INF/classes /app

ENTRYPOINT ["java","-cp","app:app/lib/*","org.springframework.samples.petclinic.PetClinicApplication"]