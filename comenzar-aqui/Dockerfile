FROM alpine

# crea el directorio y a partir de aqui ese es el destino
WORKDIR /app
# add es mas poderoso que Copy pq me permite añadir urls
COPY myapp.sh .

#Evitar el uso de 2 run seguidos
RUN ls /app && chmod +x myapp.sh && apk add --update bash

# comando que va a correr o mantener el contenedor

#CMD [ "./myapp.sh" ]

ENTRYPOINT [ "bash", "myapp.sh" ]

#CMD parametros. Este comando puede ser sobreescrito desde la linea de
#ejecucion del comando docker run
#ENTRYPOINT parametros
