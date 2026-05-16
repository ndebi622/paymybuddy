#image de base distribution java amazone,et alpine distribution legere linux
FROM amazoncorretto:17-alpine
#informations sur le maintenancier
LABEL maintainer="ndoumbendebi@gmail.com" \
      description="PayMyBuddy Backend"
#Creation du repertoire de travail de l’application dans notre container
WORKDIR app/
#copie du fichier .jar de l’app et renommage en buddyapp.jar
COPY target/paymybuddy.jar buddyapp.jar
#exposition du port 8080
EXPOSE 8080
#lancement de l’application
CMD ["java", "-jar", "buddyapp.jar"]
